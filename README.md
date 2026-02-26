
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

## Clarification : Dark Web et légalité

Le dark web ne désigne pas une activité illégale en soi.

Il s'agit d'un ensemble de services accessibles uniquement via des réseaux anonymisants
comme Tor, utilisant des adresses en .onion.

Le dark web peut contenir :

- Des services légitimes (journalisme, lanceurs d’alerte, protection de la vie privée)
- Des outils de sécurité et d’anonymisation
- Des forums communautaires
- Des plateformes de communication protégées

Cependant, comme tout espace numérique anonyme, il peut également
être utilisé à des fins illégales.

Ainsi, l’illégalité ne provient pas du réseau Tor ou du dark web en lui-même,
mais de l’usage qui en est fait.

---

## Accès au Dark Web

L’accès au dark web nécessite l’utilisation d’un réseau anonymisant,
comme le réseau Tor.

Les services hébergés sur le réseau Tor utilisent des adresses spécifiques
se terminant par l’extension ".onion".

Ces adresses ne sont pas accessibles depuis un navigateur classique
(Chrome, Edge, Firefox standard) et nécessitent l’utilisation
du navigateur Tor pour être consultées.

Ainsi, l’accès aux services en .onion confirme que la navigation
s’effectue sur le réseau Tor (dark web).

----

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

<p align="center">
  <img src="Capture_ecran-configuration-tor.PNG" width="700">
</p>


<pre>
wget https://www.torproject.org/dist/torbrowser/linux/tor-browser-linux64-*.tar.xz
tar -xf tor-browser-linux64-*.tar.xz
cd tor-browser
./start-tor-browser.desktop
</pre>

<p align="center">
  <img src="Capture_ecran_téléchargement_navigateur_tor.PNG" width="700">
</p>

----

Méthode alternative   

sudo apt update  
sudo apt install torbrowser-launcher   

---

## Fonctionnement du circuit Tor

Lorsque l’utilisateur se connecte à un service .onion,
le trafic est routé à travers plusieurs relais (nœuds)
afin de préserver l’anonymat.

Le circuit Tor est composé généralement de :
- Un nœud d’entrée (Guard Node)
- Un relais intermédiaire
- Un nœud de sortie (dans le cas d’un site classique)

<p align="center">
  <img src="capture_ecran_circuit_tor.png" width="800">
</p>

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

![DuckDuckGo Tor](Capture_ecran_tor_duckduckgo_accueil.PNG)


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

<p align="center">
  <img src="Capture_service_email_temporaire_darkweb_tor.PNG" width="800">
</p>



<p align="center">
  <img src="Capture_analyse_formulaire_incription_darkweb_tor.PNG" width="800">
</p>

⚠️ Analyse de risque   

Risques identifiés :   
	•	Collecte potentielle de métadonnées    
	•	Exploitation JavaScript   
	•	Faux miroir .onion   
	•	Tracking de session   
	•	Téléchargement de fichiers malveillants   

Décision : arrêt volontaire avant toute interaction ou saisie de données.


⸻  

### Exemple d’accès à un lien .onion

La capture ci-dessous illustre l’accès à un service via une adresse en `.onion`, accessible uniquement à travers le réseau Tor.

Les services `.onion` ne sont pas indexés par les moteurs de recherche classiques et nécessitent l’utilisation de Tor Browser.

### Risques potentiels associés

L’accès à un lien `.onion` inconnu peut présenter plusieurs risques :

- Absence d’identification claire de l’opérateur du service
- Présence possible de contenus malveillants
- Risques de phishing ou de collecte de données
- Téléchargement potentiel de fichiers infectés
- Exposition à des contenus illicites

Il est donc recommandé :

- D’utiliser un environnement isolé (machine virtuelle)
- De ne pas interagir avec des formulaires sensibles
- De ne télécharger aucun fichier
- De ne divulguer aucune donnée personnelle

Cette analyse a été réalisée dans un cadre académique et observationnel uniquement.

Il ne s’agit pas d’une action intrusive, mais d’une consultation passive dans un cadre académique.    

<p align="center">
  <img src="capture_ecran_exemple_lien_onion_darkweb.png" width="800">
</p>

⸻   


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


