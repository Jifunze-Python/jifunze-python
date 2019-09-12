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

## Types de données

Le Python est un langage dynamiquement typé. Ce qui veut dire que vous n'avez pas besoin de renseigner le type d'une variable à sa declaration, Python déduit automatiquement le type de la variable en fonction de son contenu. Contrairement à des langages comme le C ou Java, ou il faut explicitement spécifier le type de la variable, et le type de la variable reste le meme durant l'execution du programme, en Python, une variable peut changer de type pendant l'execution du programme sans problème.

Les types de donnees en Python sont nombreux. Nous avons:

- Les booléens (Boolean) qui sont soit vrai (True) soit faux (False). Un utilisateur est actif (True) ou pas (False).
- Les nombres qui peuvent êtres des entiers (Integer) comme l'age d'un utilisateur (25) ou des nombres décimaux (Float) comme la taille d'un utilisateur en mètres (1.80)
- Les chaines de caractères (String) qui sont une sequences de caractères alpha numériques. Le nom de l'utilisateur (Diallo) ou son téléphone (+221 33 000 00 00)
- Les listes (List) qui sont des suites de valeur ordonnées. Les notes de l'utilisateur [10, 14, 10.5, 14]
- Les tuples (Tuple) qui sont des suites de valeur ordonnées non modifiables. Les cordonnées longitude et latitude de l'adresse de l'utilisateur (-12.0000, 45.000)
- Les sets (Set) qui sont une suite de valeur unique (pas de repetition)
- Les dictionnaires (Dictionary) qui sont une suite de pair clé-valeur, chaque clé à une valeur

Nous allons d'abord des 3 premiers, booléens, nombres et chaines de caractères. Nous verrons les autres plus tard.

### Les booléens (Boolean)

Les booléens sont des types qui ne peuvent prendre que deux valeurs: vrai ou faux. En Python, deux constantes sont utilisées pour représenter ces valeurs: True pour vrai et False pour faux. Il faut bien remarquer la première est en majuscule et n'oubliez pas cela.

Les booléens sont par exemple pour savoir si un utilisateur est toujours actif ou pas, si un article est publier ou pas, ...

```python
>>> is_active = True
>>> is_published = False
>>>
```

### Les nombres (Number)

Python supporte deux types de nombres, les entiers et les décimaux. Les nombres sont pratiquement utilisés dans tout les programmes: enregistrer les scores dans un jeu, les notes d'un élève dans une application web, ...

```python
>>> age = 25
>>> height = 1.92
>>>
```

La variables age est ici de type entier alors que la variable height est de type decimal. On utilise le point pour les valeurs décimales.

Nous pouvons effectuer toutes les opérations mathématiques que nous connaissons déjà.

```python
>>> 4 + 7
11
>>> 4.0 + 7
11.0
>>> age = 25
>>> pi = 3.14
>>> age + pi
29.14
>>> 5 / 2
2.5
>>> 5 // 2
2
>>>
```

L'interpréteur nous affiche le résultat de chaque opération. Sur la dernière opération (5 // 2) le double slash (//) retourne la partie entière de la division. Et quand nous faisons une operation entre un entier et décimal, la réponse est un décimal.

Nous pouvons aussi calculer le carré:

```python
>>> 2 ** 2
4
>>> 4 ** 4
256
>>>
```

Python supporte aussi la priorité dans les opérations:

```python
>>> 4 + 4 * 4
20
>>> (4 + 4) * 4
32
>>>
```

Et pour afficher un nombre, on utilise toujours print()

```python
>>> age = 25
>>> print(age)
25
>>>
```

### Les chaines de caractères (String)

Une chaîne de caractères est simplement un ensemble de caractères alphanumériques, les uns à la suite des autres. En Python, les chaines de caractères sont délimitées par des apostrophes, simples ou double.

```python
>>> 'Ceci est une chaîne de caractères'
>>> "Ceci est une chaîne de caractères"
```

Si vous ouvrez une chaîne de caractères avec une apostrophe simple, vous la fermer avec une apostrophe simple, c'est aussi valable pour les apostrophes doubles.

Les chaines de caractères vont par exemple nous permettre d'enregistrer le nom d'un utilisateur, son telephone, ...

```python
>>> name = 'Diallo'
>>> phone = '+221 33 000 00 00'
>>> email = "user@gmail.com'
```

Nous pouvons additionner deux chaines, c'est ce qu'on appelle la concaténation, rappelez-vous en:

```python
>>> bonjour = 'Bonjour'
>>> name = 'Diallo'
>>> message = bonjour + name
>>> print(message)
BonjourDiallo
>>>
```

Oups, Houston, we got a problem. Il n'y a pas d'espaces. Eh ben il faut le rajouter:

```python
>>> bonjour = 'Bonjour'
>>> name = 'Diallo'
>>> message = bonjour + ' ' + name
>>> print(message)
Bonjour Diallo
>>>
```

Et voilà!

Mais quand utiliser une apostrophe simple ou double?

> Utiliser des apostrophes simples si votre chaîne contient des apostrophes doubles et utilisez des apostrophes doubles si votre chaîne contient des apostrophes simples.

C'est aussi simple que cela:

```python
>>> sentence1 = "Je vais à l'école"
>>> print(sentence1)
Je vais à l'école
>>> sentence2 = 'Je suis "COOL"'
>>> print(sentence2)
Je suis "COOL"
```

Et si votre chaîne contient les deux? Utiliser soit une apostrophe simple et précéder tout les apostrophes par un antislash (\) ou des doubles apostrophes et précéder toutes les doubles apostrophes par un antislash:

```python
>>> sentence1 = 'Je vais à l\'école et je suis "COOL"'
>>> print(sentence1)
Je vais à l'école et je suis "COOL"
>>> sentence2 = "Je vais à l'école et je suis \"COOL\""
>>> print(sentence2)
Je vais à l'école et je suis "COOL"
```

Et si votre chaîne fait plus d'une ligne, vous pouvez utilisez les triples apostrophes:

```python
>>> sentence = """Je vais à l'école et
    Je suis "COOL"
"""
>>> print(sentence)
Je vais à l'école et
    Je suis "COOL"
```

Nous verrons plus sur les chaines de caractères dans un autre chapitre, pour le moment nous allons nous limiter ici.

### type()
