# Dépannage — Head Tracker+Voice+Instructor

🌐 [English](troubleshooting.en.md) · [Русский](troubleshooting.ru.md) · Français · [Deutsch](troubleshooting.de.md) · [Italiano](troubleshooting.it.md)

Trouvez votre symptôme, puis suivez les étapes dans l’ordre. Si rien n’y fait, [envoyez un rapport](#envoyer-un-rapport-au-développeur).

## Installation

### « Windows a protégé votre ordinateur » — impossible de continuer
Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**. S’il n’y a pas de bouton **Exécuter quand même**, le Contrôle intelligent des applications est activé : voir [Installation, étape 2.5](install.fr.md).

### Le navigateur refuse de conserver le fichier téléchargé
Edge : **…** → **Conserver** → **Afficher plus** → **Conserver quand même**. Chrome : cliquez sur le fichier → **Télécharger le fichier non sécurisé**.

### Le premier lancement est long
Microsoft Defender analyse le nouveau programme ; cela peut prendre jusqu’à une minute. Patientez.

### L’installation indique « Le programme est lancé : fermez-le… »
Fermez le programme avec **Fichier → Quitter** (pas seulement avec le ✕ de la fenêtre), puis relancez l’installation.

## Connexion de l’iPhone

### L’application iPhone indique qu’il n’y a pas de connexion au PC
1. Le programme doit être lancé sur le PC.
2. **Câble :** branchez-le, déverrouillez l’iPhone et répondez **Se fier** s’il demande « Se fier à cet ordinateur ? ».
3. **Wi-Fi :** le PC et l’iPhone doivent être sur le même réseau.
4. Touchez **Réessayer** dans l’application.

### La connexion marchait, puis s’est arrêtée pendant le vol
1. Vérifiez le câble (ou le Wi-Fi).
2. Cliquez de nouveau sur **Démarrer** dans le programme du PC.
3. Si l’application indique une mauvaise qualité du Wi-Fi, utilisez le câble ou rapprochez-vous du routeur.

### L’iPhone semble fonctionner, mais le PC indique « visage non visible »
1. Dans le programme du PC, ouvrez **Réglages → iPhone** et choisissez à nouveau la connexion (câble ou Wi-Fi).
2. Cliquez de nouveau sur **Démarrer**.

### Avec le câble, l’iPhone n’est parfois pas trouvé
1. Débranchez puis rebranchez le câble, iPhone déverrouillé.
2. Fermez les autres programmes qui utilisent l’iPhone comme caméra ou webcam.
3. Essayez un autre câble ou une autre prise du PC.

## Suivi de tête

### La vue ne bouge pas
1. En bas de la fenêtre principale : **EN MARCHE** s’affiche-t-il en vert ? Sinon, cliquez sur **Démarrer**.
2. Dans le bloc **Vue** : est-il indiqué **visage détecté** ? Sinon, voir ci-dessous.
3. Asseyez-vous bien droit et cliquez sur **Centrer** (Ctrl+Alt+C).
4. Vérifiez que la **Pause** n’est pas activée (Ctrl+Alt+X l’active ou la désactive).

### « Visage non visible »
- L’iPhone doit être tourné vers vous, à environ une longueur de bras, sans rien entre vous et la caméra.
- Évitez une forte lumière juste derrière votre tête.
- Si vous avez caché votre visage un instant, le suivi reprend tout seul après quelques secondes.

### La vue est lente, saccadée ou trop sensible
**Profils → Réglages de la vue** → cliquez sur la courbe toute prête **Chasseur** ou **Civil**. Ajustez ensuite **Sensibilité** et **Lissage** dans la fenêtre principale.

### La vue part du mauvais côté (à gauche au lieu de droite)
Ouvrez **Profils → Réglages de la vue**. Dans la liste **Axes**, cliquez sur l’icône ⇄ à droite de cet axe (⇄ = miroir, sens inversé). Ensuite, merci de nous le [signaler](https://github.com/liaison-studio/htvi/issues/new/choose) en indiquant le nom du simulateur : le sens devrait être correct sans réglage.

### La vue se décentre peu à peu
Asseyez-vous bien droit et appuyez sur **Ctrl+Alt+C** (ou dites « recentrer la vue »). Pour une correction automatique, activez **Recentrage lent** dans **Profils → Réglages de la vue**.

## Commandes vocales

### Une commande n’est pas reconnue
1. La langue des commandes dans le programme du PC (**Réglages → Voix**) et la langue de la parole sur l’iPhone (**Réglages → Langue de la parole**) doivent être les mêmes. Si elles diffèrent, la fenêtre principale affiche un bandeau jaune.
2. Si vous utilisez le PTT, maintenez le bouton enfoncé pendant que vous parlez.
3. Parlez court, comme un pilote : « train sorti », pas une longue phrase.
4. La liste des phrases pour votre jeu se trouve dans la fenêtre **Commandes**.

### Une commande a été reconnue mais n’a rien fait dans le jeu
Cliquez sur **Échec — désactiver** sous la dernière commande. Le programme le note pour que la commande puisse être corrigée. Merci de nous le [signaler](https://github.com/liaison-studio/htvi/issues/new/choose) aussi, avec la phrase et le simulateur.

## Instructeur

### L’instructeur reste muet
Windows n’a pas de voix pour votre langue. **Paramètres Windows → Heure et langue → Voix → Ajouter des voix**, ajoutez une voix pour votre langue, puis redémarrez le programme.

### L’instructeur suit le mauvais avion
Dans le bloc **Instructeur**, choisissez l’avion vous-même au lieu de **Du jeu**.

## Envoyer un rapport au développeur
1. **Service → Rapport pour le développeur…**
2. Décrivez ce qui s’est passé.
3. Cliquez sur **Enregistrer l’archive…**. L’archive est enregistrée dans *Documents → Head Tracker Voice Instructor → Reports*.
4. Joignez-la à un [signalement de bug](https://github.com/liaison-studio/htvi/issues/new/choose) ou envoyez-la à liaison.studio.contact@gmail.com.

Le rapport ne contient ni son, ni données d’association. Le programme n’envoie jamais rien de lui-même.
