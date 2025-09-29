# Site Association

## Mise en place d'un environnement virtuelle linux

Dans un premier temps, j'ai créé un dossier association

```bash
mkdir /var/www/html/association
```
J'ai en suite créer un lien vers un dossier que j'ai créer dans mon dossier perso pour éviter de devoir travaillé en sudo à chaque fois

```bash
sudo ln -s ~/association /var/www/html/association
```

j'ai ensuite modifié le fichier 000-default.conf qui se trouve dans ```/etc/apache2/sites-available```

![Texte alternatif](images/default.png)

J'ai par la suite modifé le fichier hosts qui se trouve dans ```/etc/hosts```

![Texte alternatif](images/hosts.png)

Puis faire la même chose sur le fichier hosts sur windows qui se trouve dans ```C:/Windows/System32/drivers/etc```

![Texte alternatif](images/hostsW.png)

Pour finir, je vérifie en tapant

```bash
wslview http://association
```
