# holbertonschool-network-basics_1

**Projet éducatif Holberton School - Concepts réseau avancés**

## 📋 Description

Ce repository contient la suite des exercices du cours **networking basics** de Holberton School. Il approfondit les concepts réseau fondamentaux étudiés dans `basics_0`, en se concentrant sur l'adressage réseau, les interfaces localhost/127.0.0.1, les hôtes virtuels et la gestion des fichiers de configuration réseau.

Le projet vise à consolider la compréhension des mécanismes réseau et à introduire des concepts pratiques d'administration système.

## 🎯 Objectifs d'apprentissage

- **Maîtriser localhost et 127.0.0.1** : Interface de loopback et ses applications
- **Comprendre 0.0.0.0** : Interface wildcard et écoute sur toutes les interfaces
- **Gérer le fichier /etc/hosts** : Résolution de noms locale et redirection
- **Afficher les interfaces réseau** : Commandes d'administration et diagnostic
- **Manipuler les redirections** : Port forwarding et configuration réseau

## 🛠️ Concepts et technologies abordés

- **Interface localhost (127.0.0.1)** - Boucle locale pour tests et développement
- **Interface wildcard (0.0.0.0)** - Écoute sur toutes les interfaces disponibles
- **Fichier /etc/hosts** - Table de correspondance nom d'hôte/adresse IP
- **Interfaces réseau** - Configuration et affichage des cartes réseau
- **Port forwarding** - Redirection de ports pour services réseau

## 📁 Structure du projet

```
basics_1/
├── 0-change_your_home_IP
├── 1-show_attached_IPs
├── 2-port_listening_on_localhost
└── README.md
```

## 🚀 Exercices inclus

### Exercice 0: Change your home IP
- **Objectif** : Modifier la résolution DNS locale
- **Concepts** : Fichier /etc/hosts, redirection d'adresses
- **Script** : Configuration pour que `localhost` résolve vers `127.0.0.2` et `facebook.com` vers `8.8.8.8`
- **Applications** : Blocage de sites, tests de développement

### Exercice 1: Show attached IPs
- **Objectif** : Afficher toutes les adresses IP IPv4 actives
- **Concepts** : Interfaces réseau, commandes d'administration
- **Script** : Extraction et affichage des adresses IP configurées
- **Outils** : `ifconfig`, `ip`, filtrage avec `grep` et `awk`

### Exercice 2: Port listening on localhost  
- **Objectif** : Écouter sur un port spécifique en localhost
- **Concepts** : Interface de loopback, services réseau locaux
- **Script** : Configuration d'un service écoutant sur localhost:98
- **Applications** : Services de développement, API locales

## 📚 Concepts clés approfondis

### Interface localhost (127.0.0.1)
- **Boucle locale** : Trafic qui ne quitte jamais la machine
- **Tests et développement** : Services accessibles uniquement localement
- **Sécurité** : Isolation des services sensibles
- **Performance** : Communication ultra-rapide sans passer par la carte réseau

### Interface wildcard (0.0.0.0)
- **Écoute universelle** : Accepte les connexions sur toutes les interfaces
- **Services publics** : Serveurs web, bases de données accessibles de l'extérieur
- **Configuration flexible** : Adaptation automatique aux interfaces disponibles

### Fichier /etc/hosts
- **Résolution locale** : Priorité sur les serveurs DNS
- **Format** : `adresse_ip nom_d'hôte [alias]`
- **Cas d'usage** : Tests, développement, blocage de sites
- **Ordre de résolution** : /etc/hosts → DNS cache → serveurs DNS

## 🔧 Commandes et outils utilisés

### Affichage des interfaces réseau
```bash
# Méthodes traditionnelles
ifconfig                    # Configuration des interfaces (deprecated)
netstat -i                  # Statistiques des interfaces

# Méthodes modernes  
ip addr show               # Affichage détaillé des adresses
ip route show              # Table de routage
ss -tuln                   # Sockets en écoute
```

### Gestion du fichier hosts
```bash
# Édition du fichier hosts
sudo nano /etc/hosts
sudo vim /etc/hosts

# Vérification de la résolution
nslookup localhost
dig localhost
getent hosts localhost
```

### Tests de connectivité
```bash
# Tests locaux
ping 127.0.0.1
ping localhost
netstat -an | grep :98
ss -tuln | grep :98
```

## 💡 Applications pratiques

### Développement web
- **Environnements locaux** : Sites web en développement
- **Tests d'API** : Services REST accessibles via localhost
- **Bases de données** : Connexions locales sécurisées

### Administration système
- **Services système** : Configuration d'écoute sélective
- **Sécurité réseau** : Restriction d'accès aux services
- **Diagnostic** : Identification des services actifs

### Tests et debugging
- **Redirection de domaines** : Tests sans modifier DNS
- **Simulation d'environnements** : Reproduction de configurations
- **Isolation de services** : Tests sans impact sur le réseau

## 🎓 Contexte Holberton School

Ce projet consolide les acquis de `basics_0` en ajoutant :
- **Configuration système** : Manipulation de fichiers critiques
- **Administration réseau** : Gestion des interfaces et services
- **Sécurité** : Compréhension des implications des configurations
- **Pratique** : Scripts d'automatisation des tâches réseau

## 📋 Prérequis

- **Connaissances de base** des réseaux (basics_0 complété)
- **Administration Linux** : Édition de fichiers système avec sudo
- **Ligne de commande** : Maîtrise des outils bash
- **Concepts IP** : Compréhension des adresses et masques réseau

## 🔐 Considérations de sécurité

### Fichier /etc/hosts
- **Permissions** : Accessible uniquement en root
- **Impact système** : Affect la résolution de tous les utilisateurs
- **Précautions** : Sauvegarder avant modification

### Services en écoute
- **Interface binding** : Choisir l'interface appropriée (localhost vs 0.0.0.0)
- **Ports privilégiés** : Ports < 1024 nécessitent des privilèges root
- **Firewall** : Coordonner avec les règles de pare-feu

## 🤝 Contribution

Ce projet étant éducatif :
- Comprendre les implications de chaque configuration
- Tester dans un environnement isolé
- Documenter les modifications apportées
- Respecter les bonnes pratiques de sécurité

## 📞 Ressources utiles

- [Linux Network Configuration](https://tldp.org/LDP/nag2/x-087-2-iface.html)
- [Understanding /etc/hosts](https://www.howtogeek.com/27350/beginner-geek-how-to-edit-your-hosts-file/)
- [IP Command Cheat Sheet](https://access.redhat.com/sites/default/files/attachments/rh_ip_command_cheatsheet_1214_jcs_print.pdf)
- [Localhost vs 0.0.0.0](https://stackoverflow.com/questions/20778771/what-is-the-difference-between-0-0-0-0-127-0-0-1-and-localhost)
