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

Si tu as le meme resultat qui s'affiche, c'est que Python est deja installer sur ta machine. Tu viens d'ouvrir ce qu'on appelle l'interpreteur Python.
Sauf qu'il y a un petit probleme, dans ce livre nous allons parler que de Python 3, sauf qu'ici comme nous le montre la deuxieme ligne, nous avons Python 2.7.15, il nous faut donc la version recente de Python qui est Python 3. Pour quitter l'interpreteur, appuie simultanement sur le touches Ctrl + D.
Si ton systeme d'exploitation est recent, tu dois aussi avoir Python 3 installer dessus, pour le verifier, toujours dans ton terminal entre la commande python3

```bash
$ python3
Python 3.6.8 (default, Jan 14 2019, 11:02:34)
[GCC 8.0.1 20180414 (experimental) [trunk revision 259383]] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

Si tu as la meme reponse c'est que Python 3 est bien installer sur ton ordinateur. Sinon, il va falloir l'installer et pour cela tu vas utiliser ton gestionnaire de package apt pour Debian/Ubuntu ou dnf pour Fedora.

```bash
# Debian / Ubuntu
$ sudo apt install python3

# Fedora
$ sudo dnf install python3
```

Quand l'installation sera terminer, tu peux donc entrer la commande python3 pour confirmer que tout l'installation s'est bien passer.

## Exécuter Python en ligne de commande / Interpréteur

## Installer et configurer un éditeur de texte

## Créer un fichier Python

## Exécuter un fichier Python
