# 🚀 Roadmap Keycloak – Apprentissage en 8 Etapes

Ce projet est une **roadmap pratique** pour apprendre à maîtriser **Keycloak**, un Identity and Access Management (IAM) open-source basé sur OpenID Connect et SAML.  
L’objectif est de progresser étape par étape, depuis l’installation de base jusqu’au déploiement en production et à l’automatisation.

---

## 📅 Programme

### 🔹 Etape 1 : Mise en place & bases
- Installation (Docker / Docker Compose).
- Création d’un **Realm**, d’un **Client** et de **Utilisateurs**.
- Test d’authentification via **Postman**.
- Intégration simple avec une application de test (Node.js, Spring Boot, etc.).

**🎯 Exercice :** protéger une petite app avec Keycloak et afficher le token utilisateur après login.

---

### 🔹 Etape 2 : Rôles & organisation
- Différencier **Rôles Realm** et **Rôles Client**.
- Création et mapping de **Groupes**.
- Vérifier l’impact sur les tokens JWT.

**🎯 Exercice :** afficher un bouton spécial uniquement pour les utilisateurs Admin dans l’application.

---

### 🔹 Etape 3 : Claims & mappers
- Ajouter des **User Attributes**.
- Créer des **Client Scopes**.
- Utiliser des **Protocol Mappers** pour enrichir le JWT.

**🎯 Exercice :** injecter un attribut personnalisé (`department`, `team`) dans le token et le lire côté app.

---

### 🔹 Etape 4 : Flows & personnalisation
- Activer le **self-registration**.
- Vérification email et reset password.
- Création de **flows personnalisés**.
- Personnalisation de l’UI avec un **Theme**.

**🎯 Exercice :** créer un flux avec vérification d’email obligatoire + page de login custom.

---

### 🔹 Etape 5 : Fédération & SSO
- Ajouter un **Identity Provider externe** (Google, GitHub, Azure AD).
- Configurer la **User Federation** (LDAP / Active Directory).
- Mettre en place du **SSO multi-apps**.

**🎯 Exercice :** connecter deux applications différentes et tester le SSO.

---

### 🔹 Etape 6 : Sécurité avancée
- Activer le **MFA / TOTP**.
- Forcer le MFA pour certains rôles.
- Configurer les **password policies**.
- Découvrir les **Authorization Services** (ABAC/RBAC).

**🎯 Exercice :** forcer le MFA uniquement pour les utilisateurs Admin.

---

### 🔹 Etape 7 : Supervision & production
- Configurer les **logs et events**.
- Exporter les logs vers un **SIEM** (ex. Wazuh).
- Gérer la **rotation des clés (JWKS)**.
- Sécuriser Keycloak avec un reverse proxy (Nginx + TLS).

**🎯 Exercice :** déclencher une alerte SIEM après plusieurs échecs de connexion.

---

### 🔹 Etape 8 : DevOps & HA
- Sauvegarde & restauration de la base Keycloak.
- Déploiement en **cluster** (Kubernetes / Docker Swarm).
- Automatisation avec **kcadm.sh**, Terraform, Ansible, Helm.
- Concepts de **scalabilité et haute disponibilité**.

**🎯 Exercice :** script `kcadm.sh` pour créer automatiquement un Realm, un Client et un utilisateur.

---

## 📖 Ressources utiles
- [Documentation officielle Keycloak](https://www.keycloak.org/documentation)
- [Keycloak GitHub](https://github.com/keycloak/keycloak)
- [OIDC Specs](https://openid.net/developers/specs/)
- [Keycloak Docker Hub](https://hub.docker.com/r/keycloak/keycloak)

---

## 🛠️ Technologies utilisées
- **Keycloak** (IAM)
- **Docker / Docker Compose**
- **Postman**
- (optionnel) **Kubernetes**, **Terraform**, **Ansible**
- Applications de test : Node.js, Spring Boot, ou autres frameworks

---

## 📌 Objectif final
À l’issue de cette roadmap, vous serez capable de :
- Déployer et configurer Keycloak.
- Gérer les utilisateurs, rôles, groupes et permissions.
- Mettre en place un SSO multi-applications.
- Sécuriser avec MFA, policies et authorization services.
- Superviser et auditer Keycloak (logs, SIEM).
- Automatiser et industrialiser un déploiement en production.

---

✍️ N’hésitez pas à **forker** et à proposer des **améliorations** pour enrichir cette roadmap !
