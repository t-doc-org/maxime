# Introduction

## Qu'est-ce que la programmation ?

Comme cela se trouve dans le mot, la programmation consiste à créer des programmes informatiques. Il peut s'agir de programmes tels que des applications pour ordinateur comme Word ou Discord, des applications Web comme YouTube ou Twitch, des applications mobiles comme Instagram ou Whatsapp, ou encore de jeux-vidéos en 2D et 3D. Pour créer ces programmes, les informaticiens doivent communiquer à l'ordinateur les instructions à effectuer. La difficulté de cette tâche réside dans le fait qu'il n'est pas possible de parler en français à un ordinateur pour lui expliquer le déroulement d'un programme. Pour écrire un programme dans lequel l'utilisateur doit écrire son adresse email et son mot de passe, on ne peut donc pas écrire :

``` {code-block} text
:caption: Ceci n'est pas un vrai programme...
Demande à l'utilisateur d'écrire son adresse email et son mot de passe
Si la combinaison est correcte, alors affiche le message "Bienvenue"
Si ce n'est pas le cas, affiche "Mot de passe incorrect"
```

L'ordinateur est uniquement capable de comprendre des instructions très simples, écrites dans un *langage de programmation*. Dans ce cours, nous apprendrons ainsi à utiliser le langage **Python** pour communiuquer avec notre ordinateur et créer des programmes. L'exemple du programme avec l'adresse email et le mot de passe pourrait alors ressembler à cela en Python :

``` {code-block} python
:caption: Un vrai programme Python (Vous n'avez pas besoin de comprendre cela pour l'instant !)
import database_management
email = input("Email : ")
mot_de_passe = input("Mot de passe : ")
if database_management.check_password(email, mot_de_passe):
    print("Bienvenue")
else:
    print("Mot de passe incorrect")
```

## Que va-t-on apprendre à programmer avec Python ?

Théoriquement, n'importe quel programme peut être réalisé avec Python. Toutefois, tout comme l'apprenti.e cuisinier.ère commence par apprendre à couper des légumes avant de mijoter des plats élaborés, vous allez également commencer par développer des programmes simples avant de vous lancer dans le développement de programmes complexes. L'étape par laquelle passent tou.te.s les apprenti.e.s informaticien.nes est la création de *programmes consoles*. Il s'agit de programmes ne pouvant pas afficher d'images ou utiliser la souris, mais affichant uniquement du texte et pouvant interagir avec le clavier. Par exemple, la description d'un programme que vous serez amenés à créer dans ce cours est la suivante :

 *Un mini-jeu dans lequel le programme choisit un nombre aléatoire en 1 et 100. L'utilisateur doit ensuite deviner ce nombre en le moins de tentatives possible. À chaque essai, le programme dira si le nombre donné est correct, trop grand, ou trop petit.*
 
 Lorsque ce jeu sera exécuté, et qu'un utilisateur y jouera, on pourra voir le texte suivant à l'écran : 
 
```{code-block} text
Bienvenue dans le Jeu du Devin !
Je pense à un nombre entre 1 et 100. A toi de deviner quel est ce nombre !
Entre ton nombre : 50
C’est plus grand ! Essaie encore.
Entre ton nombre : 75
C’est plus petit ! Essaie encore.
Entre ton nombre : 63
C’est plus grand ! Essaie encore.
Entre ton nombre : 70
C’est plus petit ! Essaie encore.
Entre ton nombre : 67
Félicitations ! Tu as trouvé le nombre mystère en 5 tentatives !
```
 
Comme vous pouvez le constater, ce genre de programme n'affiche que du texte, et l'utilisateur ne peut interagir avec celui-ci qu'en écrivant un nombre au clavier. Derrière ce programme assez simple en apparence se cachent déjà toutefois de nombreux concepts de programmation importants. Il est ainsi crucial de maîtriser ce genre de programmes consoles avant d'aller plus loin. Une fois que vous aurez acquis des bases théoriques et pratiques solides en programmation, vous pourrez alors vous lancer dans un projet de développement d'un petit jeu vidéo en 2D.

## Installation et prise en main de Thonny

Pour débuter à programmer, vous aurez besoin d'un éditeur de texte, pour écrire les instructions, ainsi que d'un interpréteur Python. Bien que les deux logiciels puissent être installés indépendamment, il est plus pratique d'installer un *Environnement de Développement Intégré* (*EDI*) qui combine les deux et intègre d'autres fonctionnalités très pratiques. Dans ce cours, nous utiliserons l'EDI *Thonny* qui est très bien adapté pour commencer la programmation. Vous pouvez télécharger ce logiciel pour Windows, Mac, et Linux depuis le site [thonny.org](https://thonny.org). Une fois le logiciel installé, si celui-ci est en anglais et que vous souhaitez changer la langue, vous pouvez le faire en cliquant sur *Tools* $\rightarrow$ *Options\...* Puis en choisissant la langue souhaitée dans le menu déroulant. Dans le menu *Affichage*, vous pouvez activer l'option *Variables* et désactiver l'option *Assistant*. Votre fenêtre devrait contenir les trois régions suivantes :


![image](images/thonny.png)


1.  *Éditeur de code*. C'est dans cette fenêtre que vous écrirez votre code en Python.

2.  *Console*. C'est ici que vous verrez le texte de vos programmes, comme l'exemple du jeu du Devin.

3.  *Variables*. Cette zone permettra de consulter l'état des variables de votre programme (voir chapitre 2).

Pour tester que votre installation est fonctionnelle, vous allez pouvoir écrire votre première ligne de code dans l'éditeur de code. Recopiez le code suivant en faisant bien attention de respecter les minuscules sur le mot `print`.

``` {code-block} python
:caption: Premier exemple de programme Python
print("Hello World !")
```

Vous pouvez ensuite cliquer sur le petit bouton vert avec un petit triangle blanc (ou appuyer sur F5). Ceci aura pour effet d'exécuter votre code. Si tout se passe normalement, vous devriez voir apparaître le texte `Hello World !` dans la console. Ce n'est pas encore très impressionnant, mais vous venez d'écrire et d'exécuter votre premier programme !
