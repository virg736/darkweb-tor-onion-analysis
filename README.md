# 🌐 Dark Web - Analyse académique d’un service .onion via Tor
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
```bash
wget https://www.torproject.org/dist/torbrowser/linux/tor-browser-linux64-*.tar.xz
tar -xf tor-browser-linux64-*.tar.xz
cd tor-browser
./start-tor-browser.desktop
```
</pre>


