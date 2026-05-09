# Inventera

<p align="center">
  <img src="https://github.com/user-attachments/assets/ccc9fdd6-cefa-4d98-a2ce-c587088ed639" width="700" alt="Inventera logo" />
</p>

## 🔹 Aperçu du projet
**Inventera** est une application de gestion d’inventaire multi-tenant conçue pour aider les entreprises à suivre, gérer et analyser leurs stocks, produits et partenaires commerciaux au sein d’une plateforme centralisée.

Le système se compose de deux parties principales :
- un backend Java Spring Boot sécurisé avec authentification JWT,
- un frontend React.js moderne et responsive.

---

## 🚀 Fonctionnalités principales
- Gestion des produits et des catégories
- Gestion des partenaires commerciaux et des entreprises
- Création et suivi des transactions d’achat/vente
- Suivi des stocks et des niveaux de réapprovisionnement
- Authentification, autorisation et gestion des rôles
- Paiements Stripe avec webhook
- Téléversement d’images via Cloudinary
- Notifications par email et réinitialisation de mot de passe
- Tableau de bord analytique et pages de reporting

---

## 🧱 Architecture du projet
- `backend/` : API REST sécurisée en Spring Boot
- `frontend/` : application client construite avec React.js
- `frontend/src/` : composants React, pages, services et styles
- `backend/src/main/java/` : contrôleurs, services, modèles, repositories et configurations

---

## 🛠️ Stack technique
### Backend
- Java 21
- Spring Boot 3.3.5
- Spring Data JPA
- Spring Security
- Spring Validation
- Spring Mail + Thymeleaf
- JWT pour l’authentification
- MySQL comme base de données
- Cloudinary pour le stockage d’images
- Stripe pour le traitement des paiements
- AWS SDK S3 (configuration possible pour stockage complémentaire)
- ModelMapper pour la transformation DTO/entité
- Lombok pour la simplification du code

### Frontend
- React 18
- React Router Dom 6
- Axios pour les appels API
- Recharts pour les graphiques
- Tailwind CSS / PostCSS pour le design responsive
- Lucide React pour les icônes
- Crypto-js pour le chiffrement côté client

---

## ⚙️ Installation & exécution
### Backend
1. Copier `backend/src/main/resources/application.properties.example` en `backend/src/main/resources/application.properties`
2. Configurer les variables de connexion MySQL et les clés Stripe / Cloudinary
3. Lancer l’API :
```bash
cd backend
./mvnw spring-boot:run
```

### Frontend
1. Installer les dépendances :
```bash
cd frontend
npm install
```
2. Lancer l’application React :
```bash
npm start
```

---

## 🔧 Variables d’environnement recommandées
### Backend
- `SPRING_DATASOURCE_URL`
- `SPRING_DATASOURCE_USERNAME`
- `SPRING_DATASOURCE_PASSWORD`
- `STRIPE_API_KEY`
- `STRIPE_WEBHOOK_SECRET`
- `CLOUDINARY_CLOUD_NAME`
- `CLOUDINARY_API_KEY`
- `CLOUDINARY_API_SECRET`
- `JWT_SECRET`
- `MAIL_USERNAME`
- `MAIL_PASSWORD`

### Frontend
- `REACT_APP_API_BASE_URL`

---

## ✅ Bonnes pratiques de développement
- Utiliser Git pour le versioning
- Séparer les branches par fonctionnalité
- Valider les schémas et les DTO côté backend
- Gérer les erreurs API côté frontend
- Tester les endpoints critiques et les flux de paiement

---

## 📝 Notes
- Ce projet est conçu pour être extensible et peut être adapté à des environnements cloud.
- La configuration de la base de données se fait via le fichier `application.properties`.
- Les images se téléchargent en externe via Cloudinary pour optimiser les performances.

---

## 📁 Structure des dossiers
- `backend/` : service Java Spring Boot
- `frontend/` : application React
- `frontend/public/` : ressources statiques
- `frontend/src/pages/` : pages principales du client
- `backend/src/main/java/com/phegondev/InventoryMgtSystem/` : code métier backend

---

## 💡 Contribution
Les contributions sont bienvenues :
1. Créer une issue décrivant le besoin
2. Ouvrir une branche dédiée
3. Soumettre une pull request claire avec des tests lorsque c’est possible

---

## 📄 Licence
Ce projet peut être documenté ici selon la licence choisie.


