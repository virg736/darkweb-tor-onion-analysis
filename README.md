
<h1 align="center">🌐 Dark Web - Analyse académique d'un service .onion via Tor</h1>

## 📌 Description du projet

Ce projet présente une analyse académique d’un service accessible via le réseau Tor (.onion), réalisée dans un environnement virtualisé et isolé.

L’objectif n’était pas d’interagir avec le service, mais de :

- Comprendre le fonctionnement de l’accès aux services .onion
- Appliquer une méthodologie cybersécurité rigoureuse
- Documenter chaque étape de manière structurée
- Analyser les risques associés à la navigation sur le Dark Web

Aucune donnée personnelle n’a été saisie.  
Aucun téléchargement n’a été effectué.

---

## Objectifs pédagogiques

- Comprendre le fonctionnement du réseau Tor
- Mettre en place un environnement d’analyse sécurisé
- Étudier le comportement d’un service .onion
- Identifier les risques techniques associés
- Documenter une démarche d’investigation responsable

---

## Sécurisation de l’environnement

### Machine hôte

- Windows sans données sensibles
- VPN Proton activé avant connexion Tor
- Aucune activité parallèle durant l’analyse

### Machine virtuelle (VirtualBox – Debian)

- Mode réseau : NAT (pas de Bridge)
- Aucun dossier partagé entre hôte et VM
- Presse-papiers bidirectionnel désactivé
- Glisser-déposer désactivé
- Aucun périphérique USB monté
- Snapshot réalisé avant navigation
- Absence de données personnelles dans la VM

Cette configuration limite les risques en cas de contenu malveillant.

---

## ⚙️ Installation de Tor Browser

### Méthode manuelle

<pre>
wget https://www.torproject.org/dist/torbrowser/linux/tor-browser-linux64-*.tar.xz
tar -xf tor-browser-linux64-*.tar.xz
cd tor-browser
./start-tor-browser.desktop
</pre>

----

Méthode alternative   

sudo apt update  
sudo apt install torbrowser-launcher   

---

🌍 Accès aux services .onion   

1️⃣ Connexion via Tor Browser   
	•	Connexion au réseau Tor   
	•	Vérification du circuit Tor   
	•	Observation des nœuds (garde, relais, sortie)   

2️⃣ Utilisation d’un moteur de recherche .onion   
	•	Accès à la version .onion de DuckDuckGo   
	•	Recherche via mots-clés liés aux services Dark Web   
	•	Consultation d’articles référençant des services .onion   
	•	Ouverture directe d’un service identifié   

⸻   

 Service analysé   

Service d’e-mail temporaire accessible via Tor.   

Caractéristiques observées :   
	•	Interface minimaliste    
	•	Création de compte possible   
	•	Aucune vérification d’identité   
	•	Conservation des messages limitée   
	•	Fonctionnement basé sur l’anonymat   

Aucune interaction sensible n’a été réalisée.   

⸻  

 Analyse technique   

Le processus correspond à une navigation anonyme standard via Tor :   
	•	Routage via plusieurs nœuds   
	•	Chiffrement multi-couches   
	•	Accès à un service caché (.onion)   

Il ne s’agit pas d’une action intrusive, mais d’une consultation passive dans un cadre académique.    

⸻   

⚠️ Analyse de risque   

Risques identifiés :   
	•	Collecte potentielle de métadonnées    
	•	Exploitation JavaScript   
	•	Faux miroir .onion   
	•	Tracking de session   
	•	Téléchargement de fichiers malveillants   

Décision : arrêt volontaire avant toute interaction ou saisie de données.

⸻

📷 Captures d’écran

Les captures documentent :
	•	Installation de Tor
	•	Paramétrage du niveau de sécurité
	•	Visualisation du circuit Tor
	•	Accès au moteur de recherche .onion
	•	Interface du service analysé
	•	Analyse du formulaire d’inscription     

⸻

🔒 Note éthique   

Les adresses .onion ont été volontairement masquées dans les captures d’écran.   

Ce choix a été fait par éthique de cybersécurité afin de :   
	•	Ne pas diffuser d’adresses sensibles   
	•	Ne pas faciliter l’accès direct aux services analysés   
	•	Respecter une démarche responsable et professionnelle   

⸻   

📈 Axes d’amélioration futurs   

Ce projet pourrait être approfondi par :   
	•	Analyse du trafic réseau (Wireshark)   
	•	Étude détaillée des circuits Tor   
	•	Inspection des certificats   
	•	Modélisation de menace complète   
	•	Analyse des logs   
	•	Étude du fingerprinting navigateur   
	•	Mini audit technique du service   

Ces éléments n’étaient pas l’objectif initial de l’exercice.   

⸻   

🎓 Niveau estimé du projet   

Niveau : Intermédiaire   
(BTS SIO / Licence 2 / Début Bachelor Cybersécurité)   

Ce projet démontre :  
	•	Compréhension du réseau Tor  
	•	Mise en place d’un environnement isolé  
	•	Analyse de risque structurée  
	•	Démarche éthique et responsable   

⸻  

⚖️ Disclaimer  

Projet réalisé à des fins pédagogiques uniquement.  
Aucune activité illégale n’a été effectuée.   


