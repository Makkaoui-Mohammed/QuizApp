# QuizApp
Application Android écrite en Java, est conçue pour être un quiz interactif avec plusieurs questions.

Authentification (MainActivity.java) :

L'utilisateur est accueilli par l'activité principale (MainActivity) où il doit saisir un identifiant (etMail) et un mot de passe (etPassword).
Si l'identifiant est "toto" et le mot de passe est "123", l'utilisateur est redirigé vers la première question du quiz (Quiz1).
Un lien vers la page d'inscription (Register) est également disponible.
Inscription (Register.java) :

L'utilisateur peut accéder à une page d'inscription où il doit fournir une adresse e-mail (etMail), un mot de passe (etPassword), et confirmer le mot de passe (etPassword1).
Des vérifications sont effectuées pour s'assurer que tous les champs sont remplis correctement.
Une fois l'inscription réussie, l'utilisateur est redirigé vers l'activité principale (MainActivity).
Quiz (Quiz1.java à Quiz5.java) :

Chaque question du quiz est présentée dans une activité distincte (Quiz1 à Quiz5).
Chaque question possède une liste de réponses sous forme de boutons radio (rg).
L'utilisateur doit choisir une réponse, et son choix est validé en appuyant sur le bouton "Suivant" (bNext).
Les activités du quiz (Quiz1 à Quiz4) passent le score accumulé à l'activité suivante via les Intent.
La dernière question (Quiz5) redirige vers l'activité de score final (Score).
Score final (Score.java) :

L'activité de score final affiche le score total sous forme de pourcentage (tvScore).
Une barre de progression (progressBar) représente visuellement le score.
Deux boutons sont disponibles : "Logout" (bLogout) pour quitter l'application et "Try Again" (bTry) pour recommencer le quiz.
