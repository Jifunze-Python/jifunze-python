# Mettre en place de notre environnement de travail

Bienvenue dans cette première partie de ce livre. Nous allons commencer par mettre en place un environnement de travail. Nous allons donc commencer par installer Python 3, puis installer et configurer un éditeur de texte pour pouvoir écrire du code Python. Nous allons ensuite exécuter ensemble notre premier programme écrit en Python.

## Installer Python

Python comme nous l'avons vu est un langage multi-plateforme, il va donc fonctionner sur Linux, Windows et Mac. Comme je vous l'ai dit dans l'introduction, c'est beaucoup mieux si vous avez un système Linux (Debian Ubuntu, Fedora, ...). Mais si ce n'est pas le cas, il n'y a aucun problème tout ce que nous verrons ici marchera parfaitement quelque soit votre Système d'Exploitation. Passons donc à l'installation de Python.

### Linux

Par défaut, les systèmes Linux viennent déjà avec Python installer dessus. Pour vérifier si Python est installer ou pas, ouvre un terminal (Ctrl + Alt + T) et entre la commande python

```bash
$ python
Python 2.7.15+ (default, Nov 27 2018, 23:36:35)
[GCC 7.3.0] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

Si tu as le meme résultat qui s'affiche, c'est que Python est deja installer sur ta machine. Tu viens d'ouvrir ce qu'on appelle l'interpréteur Python.
Sauf qu'il y a un petit problème, dans ce livre nous allons parler que de Python 3, sauf qu'ici comme nous le montre la deuxième ligne, nous avons Python 2.7.15, il nous faut donc la version récente de Python qui est Python 3. Pour quitter l'interpréteur, appuie simultanément sur le touches Ctrl + D.
Si ton système d'exploitation est recent, tu dois aussi avoir Python 3 installer dessus, pour le verifier, toujours dans ton terminal entre la commande python3

```bash
$ python3
Python 3.6.8 (default, Jan 14 2019, 11:02:34)
[GCC 8.0.1 20180414 (experimental) [trunk revision 259383]] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

Si tu as la meme réponse c'est que Python 3 est bien installer sur ton ordinateur. Sinon, il va falloir l'installer et pour cela tu vas utiliser ton gestionnaire de package apt pour Debian/Ubuntu ou dnf pour Fedora.

```bash
# Debian / Ubuntu
$ sudo apt install python3

# Fedora
$ sudo dnf install python3
```

Quand l'installation sera terminer, tu peux donc entrer la commande python3 pour confirmer que tout l'installation s'est bien passer.

Pour les utilisateur Linux, nous allons donc utiliser la commande python3 dans ce livre, parce que c'est la commande pour pouvoir utiliser Python 3.

## Exécuter Python en ligne de commande / Interpréteur

Python vient avec un interpréteur dynamique qui s'execute dans un terminal et qui nous permet d'executer du code Python sans avoir à créer un fichier. Pour lancer l'interpréteur, sur Linux il faut rentrer la commande Python 3

```bash
$ python3
Python 3.6.8 (default, Jan 14 2019, 11:02:34)
[GCC 8.0.1 20180414 (experimental) [trunk revision 259383]] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

Remarquez bien les trois chevrons >>> que nous avons tout en bas, c'est devant ces trois chevrons que nous allons écrire notre code Python. Pour valider ce que nous aurons écris, on appuie juste sur la touche Entrer. Amusons nous un peu avec cet interpréteur, nous allons faire un peu de calcul. Appuyez sur Entrer après chaque opération:

```bash
$ python3
Python 3.6.8 (default, Jan 14 2019, 11:02:34)
[GCC 8.0.1 20180414 (experimental) [trunk revision 259383]] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 3 + 2
5
>>> 3 * 2
6
>>> 6 / 2
3.0
>>>
```

Nous vous inquiétez pas pour la dernière réponse nous y reviendrons, mais ce que vous allez remarquer, c'est qu'à chaque fois que vous appuyez sur Entrer, l'interpréteur nous affiche la réponse sur une nouvelle ligne et affiche les 3 chevrons sur la ligne suivante. C'est ça l'interpréteur au fait, notre code est executer au fur et à mesure, ligne par ligne. Nous allons beaucoup l'utiliser dans ce livre pour écrire de petits programmes. Mais plus notre code évoluera, l'interpréteur ne fera plus l'affaire, il faudra donc créer des fichiers Python. Il faut savoir que l'interpréteur retient notre code tant qu'il est ouvert, dès que nous quittons l'interpréteur (avec Ctrl + D ou exit()), il oublie tout, meme si vous revenez après il ne s'en souviendra pas.

Pour créer et modifier des fichier Python, il nous faut un éditeur de code. Voyons tout de suite comment en installer un.

## Installer et configurer un éditeur de texte

## Créer un fichier Python

## Exécuter un fichier Python
