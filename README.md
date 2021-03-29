# Présentation

Lien du repository du projet : https://github.com/L3-Info-Miage-Universite-Cote-D-Azur/pl2020-plpld  


Ce répertoire contient une copie de mon projet de licence dont le sujet était le suivant : 

![Sujet](https://github.com/Ossama98/Projet-de-licence-Android/blob/master/sujet.png)
![Evo1](https://github.com/Ossama98/Projet-de-licence-Android/blob/master/Evolution1.png)
![Evo2](https://github.com/Ossama98/Projet-de-licence-Android/blob/master/Evolution2.png)

Le serveur se trouve dans java/serveur et le client dans AndroidApp , la partie commun se trouve dans java/commun  

Vous pouvez voir la participation et commit du projet dans l'onglet "contributors". 

### Ce projet a eu une soutenance : [les diapositives](https://github.com/Ossama98/Projet-de-licence-Android/blob/master/Soutenance.pdf)


# pl2020-plpld

## Liste des itérations

![Model](https://github.com/L3-Info-Miage-Universite-Cote-D-Azur/pl2020-plpld/blob/master/documentation/IHM/IHM%20final.jpg)

### Itération 1:
	Mise en place de l'environnement de travail (projet Android Studio, README.md, pom.xml...).
 	Création d’un serveur.
Création d’une classe « Identité » qui implémente l’interface « ToJSON » afin d’identifié la personne qui se connecte au serveur.
Création d’une classe « Net » qui permet de définir les messages entre le client et le serveur
Création de plusieurs classes (Connexion, EcouteurDeReseau, EcouteurDeBouton) afin de permettre la communication client-serveur
Création d’un bouton qui affiche un texte lorsque l’on clique dessus (à la prochaine itération le bouton enverra un signal au serveur, qui lui dira alors d'afficher un message).

### Itération 2
	Création d'une interface graphique côté client en se basant sur nos maquettes IHM.
	Création d'une classe "Métiers" coté serveur et client qui représente une matière (Chimie, Physique, ...).
	Création d'une constante "Choix" qui contient les choix du client (les matières choisies).
	Modification de plusieurs classes pour permettre le lien entre le client et le serveur.
	Ajout des dernières maquettes IHM.
	Mise en place d'une validation des choix lors du clic sur le bouton "valider"

### Itération 3:
	Sélection multiple d'UE désormais possible
	Les UE sont désormais catégoriser par disciplines via une ExpandableListAdapter
	L'interface graphique et son agancement ont été améliorée
	Les classes communes au serveur et au client ont été mises en commun
	Liste des itérations et IHM mise à jour en conséquence
	A noter : présence d'un bug menant parfois à l'affichage multiple de certains noms d'UE lors du déroulement d'une catégorie, il sera corrigé à la 		prochaine itération.
	
### Itération 4:
	-Création d’un écran d’accueil.
	-Mise en place d’une barre de progression composé des 4 semestre afin de sélectionner les matières semestre par semestre.
	-Modification du serveur pour permettre l’envoie de la liste des matières au client.
	-Modification du client afin qu’il reçoive la liste des matières émis par le serveur (Ceci est valable pour le semestre 1, pour les autres semestres la liste des matières est toujours en local (Ceci sera modifié lors de la prochaine itération)).
	-Mise à jour des IHM.
	
### Itération 5:
	 Création d'un écran récapitulatif.
	 Nouveau système de sélections des UE :
	Ajout d'un fichier "Prerequis.txt" qui contient les prérequis pour chaque matières.
	Mise en place d'un graphe orienté pour la sélection des UE en fonction des prérequis.
	Restriction du nombre d'UE a choisir par semestre.
	Interdiction de sélectionner plusieurs fois la même UE.
	 Modification du client afin qu'il reçoive la liste des matières émis par le serveur (ceci est valable pour tout les semestres).
	 Simplification des SemestreActivity grâce à l'héritage.
	

### Itération 6:
	Correction du bug a l'écran récapitulatif des UE.
	 Découpage de la partie serveur en 3 sous classes : "GestionnaireDeFichiers", "GestionnaireDeReseau" et "Serveur".
	 Création d'un écran d'inscription (avec enregistrement de l'utilisateur coté serveur).
	 Création d'un popup de connexion avant de démarrer un parcours.
	 Création d'une barre de recherche des UE (non fonctionnel pour le moment).
	 Possibilité de revenir en arrière sur la sélection en cliquant sur le semestre souhaité sur la barre de progression.
	 Simplification des SemestreActivity grâce à l'héritage.


### Itération 7:
	Ajout des matières du S3 et S4 avec les prérequis.
	 Ajout d'un ToolBar avec un SearchView (pas encore fonctionnel).
	 Possibilité que le client recommence son parcours depuis le récap (prochainement le client reviendra sur le semestre 4, ce qui lui permettra de ne pas recommencer un parcours en entier).
	 Possibilité que le client puisse partager son parcours via courriel.
	 Possibilté d'enregistrer le parcours du client coté serveur.
	 Création d'un bouton de confirmation (pour que le client puisse confirmer son parcours et l'envoyer au serveur).
	 Création d'une exception avec message d'erreur si le serveur ne répond pas.
	

### Itération 8:
	Le client/serveur fonctionne désormais par évenements.
	 Ajout d'un message d'erreur lorsque l'utilisateur entre une mauvaise combinaison d'identifiants.
	 Modification des classes "Serveur" et "GestionnairedeRéseau" afin que les socketIOClient soient dans la classe "Serveur".
	 Amélioration de la SearchView.
	 Mise en place de parcours prédéfini (pour le moment seul le parcours Informatique est disponible).
	 Mise a jour du fichier des prérequis.

### Itération 9:
	 Restructuration de la classe serveur.
	 Possibilité de faire des parcours partiels.
	 Finalisation de la barre de recherche.
	 Amélioration de l'interface graphique.

### Itération 10:
	Parcours préconçus améliorés.
	 Amélioration de la searchView.
	 Ajout d'une fonctionnalité mot de passe oublié.
	 Création d'un menu d'accueil.
	 Création d'une fonctionnalité de consultation des parcours des autres étudiants.
	 Description des UE.
	 Système de notification si les prérequis changent.
	 Saisie prédective du numéro d'étudiant lors de la connexion.
	 Session persistance de l'étudiant s'il ne se déconnecte pas.
	 Amélioration de l'interface graphique.
	 Ajout de la javadoc, suppression des imports inutiles.
	 Dernier ajout dans les fichier de ressources.
