# holbertonschool-network-basics_0

**Projet éducatif Holberton School - Fondamentaux des réseaux informatiques**

## 📋 Description

Ce repository contient les exercices et projets du cours de **networking basics** de Holberton School. Il couvre les concepts fondamentaux des réseaux informatiques, avec un focus particulier sur le **modèle OSI**, les protocoles **TCP/UDP**, et les bases de la communication réseau.

Le projet se concentre sur la compréhension théorique et pratique des mécanismes qui permettent aux ordinateurs de communiquer entre eux à travers les réseaux.

## 🎯 Objectifs d'apprentissage

- **Comprendre le modèle OSI** : Les 7 couches et leur rôle dans la communication réseau
- **Maîtriser les protocoles de transport** : TCP et UDP, leurs différences et utilisations
- **Analyser la couche réseau** : IP et ICMP, adressage et routage
- **Appréhender les concepts réseau** : Topologies, équipements, et architectures
- **Développer l'esprit critique** : Analyser et résoudre des problèmes réseau

## 🛠️ Technologies et protocoles abordés

- **Modèle OSI** - Framework de référence pour la communication réseau
- **TCP (Transmission Control Protocol)** - Protocole de transport fiable
- **UDP (User Datagram Protocol)** - Protocole de transport rapide
- **IP (Internet Protocol)** - Protocole de la couche réseau
- **ICMP (Internet Control Message Protocol)** - Gestion des messages d'erreur

## 📁 Structure du projet

```
basics_0/
├── 0-OSI_model
├── 1-types_of_network
├── 2-MAC_and_IP_address
├── 3-UDP_and_TCP
├── 4-TCP_and_UDP_ports
├── 5-is_the_host_on_the_network
└── README.md
```

## 🚀 Exercices inclus

### Exercice 0: OSI Model
- **Objectif** : Comprendre les bases du modèle OSI
- **Concepts** : 7 couches, organisation hiérarchique, rôle de chaque couche
- **Questions** : QCM sur la définition et l'organisation du modèle OSI

### Exercice 1: Types of Network  
- **Objectif** : Différencier les types de réseaux
- **Concepts** : LAN, WAN, Internet, topologies réseau
- **Applications** : Classification des réseaux selon leur portée

### Exercice 2: MAC and IP Address
- **Objectif** : Comprendre l'adressage réseau
- **Concepts** : Adresses MAC (couche 2), adresses IP (couche 3)
- **Différenciation** : Adressage physique vs logique

### Exercice 3: UDP and TCP
- **Objectif** : Maîtriser les protocoles de transport
- **Concepts** : Protocoles avec/sans connexion, fiabilité vs rapidité
- **Comparaison** : Avantages et inconvénients de chaque protocole

### Exercice 4: TCP and UDP Ports
- **Objectif** : Comprendre le concept de ports
- **Concepts** : Multiplexage, services réseau, ports bien connus
- **Applications** : Association ports/services (HTTP, SSH, DNS, etc.)

### Exercice 5: Is the Host on the Network
- **Objectif** : Utiliser les outils de diagnostic réseau
- **Concepts** : ICMP, ping, connectivité réseau
- **Pratique** : Script bash pour tester la connectivité

## 📚 Concepts clés du modèle OSI

### Les 7 couches (du bas vers le haut)

1. **Couche Physique** - Signaux électriques, optiques, radio
2. **Couche Liaison** - Trames, détection d'erreurs, MAC
3. **Couche Réseau** - Routage, adressage IP, ICMP
4. **Couche Transport** - TCP/UDP, ports, fiabilité
5. **Couche Session** - Établissement de sessions
6. **Couche Présentation** - Chiffrement, compression
7. **Couche Application** - HTTP, FTP, SMTP, DNS

### Caractéristiques importantes

- **Framework conceptuel** : Le modèle OSI est un modèle de référence
- **Interopérabilité** : Permet la communication entre systèmes différents
- **Séparation des responsabilités** : Chaque couche a un rôle spécifique
- **Encapsulation** : Les données transitent en ajoutant des en-têtes

## 🔧 Outils utilisés

- **Bash** - Scripts pour les exercices pratiques
- **Commandes réseau** - ping, netstat, ss
- **Outils de diagnostic** - Pour analyser la connectivité
- **Documentation** - Man pages et ressources en ligne

## 📋 Prérequis

- **Connaissances de base** en systèmes Linux/Unix
- **Compréhension basique** des ordinateurs et de l'internet
- **Capacité de lecture** de documentation technique
- **Esprit logique** pour l'analyse des problèmes réseau

## 🎓 Contexte Holberton School

Ce projet fait partie du cursus **System Engineering & DevOps** de Holberton School et vise à :
- Établir les bases solides en networking
- Préparer aux concepts avancés (sécurité, cloud, DevOps)
- Développer les compétences de troubleshooting réseau
- Comprendre l'infrastructure sous-jacente d'internet

## 📊 Évaluation

Les exercices sont évalués sur :
- **Compréhension théorique** des concepts réseau
- **Précision des réponses** aux questions techniques
- **Qualité du code** pour les scripts bash
- **Documentation** et explications fournies

## 🤝 Contribution

Ce projet étant à des fins éducatives :
- Respecter l'intégrité académique
- Favoriser la compréhension plutôt que la copie
- Partager les ressources d'apprentissage utiles
- Encourager les discussions techniques constructives

## 📞 Resources utiles

- [OSI Model - Cloudflare](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)
- [TCP/IP Guide](https://www.tcpipguide.com/)
- [RFC Documents](https://www.rfc-editor.org/) - Standards internet officiels
- [Wireshark](https://www.wireshark.org/) - Analyseur de paquets réseau

---