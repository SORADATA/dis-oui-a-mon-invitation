# 💌 Dis Oui — L'invitation à un date qu'on ne peut pas refuser

**Dis Oui** est une mini-application web interactive et ludique permettant de créer une invitation personnalisée (pour un date, une sortie, ou un verre) avec une particularité amusante : **le bouton "Non" s'échappe quand on essaie de cliquer dessus.**

Une fois l'invitation configurée, un lien unique est généré pour être envoyé (par WhatsApp, SMS, etc.). Quand la personne accepte et choisit ses options (lieu, heure), un email de confirmation est automatiquement envoyé à l'organisateur.

## ✨ Fonctionnalités

* 🎨 **Créateur d'invitation (Interface 1) :**
  * Personnalisation du prénom du destinataire.
  * Sélection d'activités (principales et alternatives) avec ajout de descriptions.
  * Sélection de créneaux horaires personnalisables.
  * Génération instantanée d'un lien unique basé sur les paramètres d'URL (pas de base de données requise).
* 💌 **Réception de l'invitation (Interface 2) :**
  * Animation d'ouverture d'enveloppe.
  * **Dark pattern humoristique :** Le bouton "Non" fuit le curseur ou le doigt de l'utilisateur (avec compteur de tentatives).
  * Sélection finale du créneau et de l'activité.
* 🚀 **Notifications par Email (Sans Backend) :**
  * Utilisation de l'API AJAX de [FormSubmit](https://formsubmit.co/) pour envoyer la réponse directement sur la boîte mail de l'organisateur.

## 🛠️ Technologies utilisées

* **Frontend :** HTML5, CSS3, JavaScript (Vanilla - sans framework).
* **Backend :** 100% Serverless. Le transfert de données se fait via les paramètres d'URL (`URLSearchParams`).
* **Mailing :** API FormSubmit (avec un fallback sur Formspree).

## 🚀 Installation & Déploiement

Ce projet ne nécessite aucun serveur pour fonctionner. Il peut être hébergé gratuitement sur **GitHub Pages**, **Vercel** ou **Netlify**.

1. **Cloner le dépôt :**
   ```bash
   git clone [https://github.com/ton-nom-utilisateur/dis-oui.git](https://github.com/ton-nom-utilisateur/dis-oui.git)