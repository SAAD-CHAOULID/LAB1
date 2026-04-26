🧪 LAB 1 — Initialisation de l’environnement Mobexler
1. 🎯 Objectif

Ce laboratoire a pour objectif la mise en place d’un environnement de test pour la sécurité des applications mobiles.

Le travail consiste à préparer une machine virtuelle Mobexler, configurer le réseau et établir la connexion avec un appareil Android.

2. 🧰 Prérequis
VirtualBox installé
Machine virtuelle Mobexler importée
Outil ADB disponible
Appareil Android ou émulateur
3. ⚙️ Déroulement
3.1 🔐 Accès à la machine virtuelle

Après le démarrage de la machine virtuelle Mobexler, la connexion s’effectue avec les identifiants suivants :

Utilisateur : mobexler
Mot de passe : mobexler

<img width="1209" height="524" alt="image" src="https://github.com/user-attachments/assets/6bc80332-c62b-4e0f-bebe-93485c9bd155" />

3.2 🌐 Test de connectivité réseau

La vérification de l’accès à Internet se fait à l’aide de la commande suivante :

ping -c 2 8.8.8.8
<img width="686" height="224" alt="image" src="https://github.com/user-attachments/assets/8c5cc72a-df14-4870-b289-2d3b9bffb967" />

Une réponse positive indique que la connexion réseau est opérationnelle.

3.3 💾 Création d’un snapshot

Un snapshot est créé afin de conserver un état stable de la machine virtuelle.

Nom du snapshot : CLEAN_BASELINE_TP1

Ce point de sauvegarde permet une restauration rapide en cas de problème.

3.4 📱 Vérification de la connexion Android

La connexion de l’appareil Android est vérifiée avec ADB :

adb version
adb devices
<img width="694" height="247" alt="image" src="https://github.com/user-attachments/assets/918b58de-297c-46a3-9417-9f655985e5d3" />

L’appareil apparaît dans la liste des périphériques si la connexion est correctement établie.

4. ✅ Résultat attendu
Machine virtuelle Mobexler fonctionnelle
Accès Internet validé
Snapshot créé
Appareil Android détecté via ADB
