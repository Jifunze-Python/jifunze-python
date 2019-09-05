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
