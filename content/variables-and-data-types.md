# Variables et Types de données

Dans ce chapitre, nous appelons découvrir les variables, ce que c'est, comment les utiliser, les afficher mais aussi découvrir les différents types de données que vous serez emmener à utiliser en Python. Alors on commence tout de suite.

## Variables

> Une variable en programmation est un espace mémoire que l'on définit au quel on associe un nom et une valeur.

Une variable est donc composer d'un label (son nom) et d'une valeur. Les variables sont utiliser pour garder des informations (données) de notre programme durant l'execution du programme. On peut par exemple utiliser une variable pour garder le nom de notre utilisateur, son age, son adresse email et toutes les informations que vous voulez.

Pour définir une variable en Python, il faut juste renseigner son nom, suivi du signe égale (=) puis sa valeur, comme ci-dessous:

```python
>>> name = 'Diallo'
>>> age = 24
>>> email = "diallo@gmail.com"
>>> height = 1.90
>>> is_active = True
>>>
```

Nous définissons les variables juste en mettant nom de la variable, puis sa valeur. C'est aussi simple que cela. Nous allons tout de suite découvrir pourquoi d'autres valeurs sont entre griffes alors que d'autres non.

### Afficher une variable

Pour afficher quelque chose en Python, nous connaissons la fonction print(), eh ben nous allons utiliser la meme pour afficher les variables. Nous allons donc mettre la variable à afficher entre les parenthèses de la fonction.

```python
>>> print(name)
Diallo
>>> print(age)
24
>>> print(email)
diallo@gmail.com
>>> print(height)
1.90
>>> print(is_active)
True
>>>
```

Vous voyez donc que la valeur contenu dans nos variables s'affichent bien.

> Alors attention, pour afficher une variable nous ne mettons la variable dans des apostrophes comme nous l'avons vu avec l'affichage du message Hello Python tout à l'heure. Si vous mettez la variable à afficher entre des apostrophes, vous n'aurez pas le contenu de la variable, mais plutôt le contenu que vous avez mis entre les apostrophes (le nom de la variable).

Si vous faites ça par exemple:

```python
>>> print('name')
name
>>> print('age')
age
```

Vous pouvez essayer pour voir ce que ça va donner. Maintenant comment afficher une variable avec du texte, disons par exemple que nous voulons dire Bonjour à notre utilisateur.

### Concaténation

Nous allons faire ce qu'on appelle de la concaténation au fait.

> La concaténation est le fait de joindre deux chaines de caractères.

Pour faire de la concaténation, nous allons utiliser le signe plus (+) comme ceci:

```python
>>> name = 'Diallo'
>>> print('Hello ' + name)
Hello Diallo
```

Hourrraaaa, vous venez de faire votre première concaténation en Python.

Je mets un espace après le Hello avant de mettre l'apostrophe fermante, c'est pour éviter que le Hello soit coller au contenu de la variable. Voyons un exemple:

```python
>>> name = 'Diallo'
>>> print('Hello' + name)
HelloDiallo
```

Vous voyez ce que ça fait? Ne confondez surtout pas avec les espaces autour du signe plus qui sont juste là pour que le code soit plus lisible.

Essayons d'afficher une phrase comme "Bonjour Diallo, votre adresse email est le: diallo@gmail.com". Essayez de votre coté avant de lire le code:

```python
>>> name = 'Diallo'
>>> email = 'diallo@gmail.com'
>>> print('Hello ' + name + ', votre adresse email est le: ' + email + '.')
Hello Diallo, votre adresse email est le: diallo@gmail.com.
```

Voilà.

### Nomination des variables

Maintenant que nous avons vu comment définir une variable, il faut savoir qu'il y a quelques règles à suivre pour donner à vos variables. La première et celle qu'il ne faut jamais négliger, c'est qu'il faut que le nom de votre variable reflète son contenu. Qu'est ce que ça veut dire? Si vous voulez d'une variable pour enregistrer le nom de votre utilisateur par exemple, la variable va s'appeler name ou nom (utilisez plutôt la version anglaise) et nom n ou quelque chose qui n'a rien à voir avec le nom. Le nom de la variable doit toujours nous indiquer ce que la variable contient. Pourquoi? Imaginez, vous développez votre application de jeu vidéo et vous donnez des noms à vos variables comme p, n et a. Alors vous vous dites peut être que p vaut prénom, n vaut nom et a vaut age. Mais non, pour moi p vaut power, n vaut name et a vaut alive. Vous voyez deja le premier problème? On n'a pas la meme signification du contenu des variables. Mais ça c'est dans le cas ou vous partagez votre code, et c'est ce qui arrive souvent, vous serez emmener à travailler en entreprise, avec d'autres personnes. Maintenant l'autre cas, si vous laissez ce code ne serait-ce que pour pour un mois sans y toucher, le jour vous allez le reprendre je peux vous assurer que vous allez vous detester, pour de vrai. Il ne faut jamais manquer cette première règle.

En plus de cela, il y a d'autres règles à respecter:

- Le Python est sensible à la casse. name est différent de Name qui est aussi différent de NAME
- Le nom d'une variable commence toujours par une lettre ou underscore \_ (tiret du 8)
- Le nom d'une variable n'est composer que de lettres, underscore et chiffres et pas de caractères accentués pas de prénom par exemple, mais plutôt prénom. C'est l'une des raisons d'utiliser l'anglais qui n'a pratiquement de caractères accentués
- Si le nom de votre variable contient des espaces, remplacer les espaces par des underscores (prenom et nom -> prenom_et_nom)
- Le nom de votre variable ne doit pas être un [mot clé](https://www.programiz.com/python-programming/keyword-list) de Python
- Encore une fois utiliser des noms de variables clairs, qui définissent le contenu de la variable

Alors plus haut, je préconise l'utilisation de l'anglais donner des noms à vos variables, name au lieu de nom, first_name au lieu de prénom et ainsi de suite, d'abord pour éviter les caractères accentués, mais aussi parce que quand vous travaillez avec d'autres personnes qui ne sont pas français, ou que vous votre projet est open source, les personnes qui liront votre code votre code doivent tout de suite se retrouver, I mean l'anglais c'est la langue du business mondial. Et puis c'es franchement joli d'avoir des noms de variables en Anglais. Toutes les variables dans ce livre seront donc en Anglais.
