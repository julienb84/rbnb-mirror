# 🏠 AirBnB Mirror – Mobile App 🏠

![Demo GIF](public/App_AirBnb_demo.gif)

Application mobile développée avec **React Native** et **Expo**, inspirée de l’application **AirBnB**.  
Ce projet a pour objectif de reproduire les principales fonctionnalités de navigation et d’authentification d’une application de location d’appartements.

---

## 📱 Fonctionnalités

L’application est composée de plusieurs écrans :

- 🔐 **Création de compte**
- 🔑 **Connexion utilisateur**
- 🏘️ **Liste des appartements disponibles à la location**
- 🏠 **Détail d’un appartement sélectionné** avec l'intégration d'une carte indiquant sa localisation
- 📷 **Photos de l'appartement**
- 🗺️ **Carte (Apple Maps)** affichant les appartements autour de l’utilisateur
- 👤 **Profil utilisateur** avec les informations personnelles

---

## 🔐 Gestion de l’authentification

L’authentification est gérée via :

- Un **AuthContext**
- Un **AuthContextProvider** pour sauvegarder le token et l'ID de l'utilisateur et les redistribuer dans toute l'application une fois la navigation autorisée

Cette approche permet :

- un accès centralisé aux données d’authentification
- une navigation conditionnelle selon l’état de connexion
- une meilleure organisation du code

---

## 🛠️ Technologies utilisées

- **React Native**
- **Expo**
- **Expo Router**
- **React createContext**
- **Apple Maps**
- **JavaScript**

---

## 📂 Structure du projet

```
app/
├── layout.js (Stack layout)
├── (auth)/
│ ├── layout.js (Stack layout)
│ ├── index.js
│ └── signup.js
└── main/
├── layout.js (Tabs layout)
├── home/
│ ├── layout.js (Stack layout)
│ ├── rooms.js
│ ├── rooms.js
│ └── pictures.js
├── map.js
└── profile.js
```

---

## 🚀 Installation

### Prérequis

- [Expo](https://expo.dev) installé sur la machine

### Étapes

1. Cloner le dépôt :

```bash
git clone https://github.com/JulienBCHZ/rbnb-mirror.git
```

2. Installer les dépendances :

```bash
npx expo install
# ou
yarn install
```

3. Lancer le projet en mode développement :

```bash
npx expo
# ou
yarn start
```

Appuyer sur la touche `i` pour lancer un simulateur iOS ou appuyer sur la `a` pour lancer un simulateur Android.
Scanner le QR Code affiché dans le terminal avec un appareil iOS ou Android pour ouvrir l'application Expo Go.

---

## 🎯 Objectifs du projet

- Mettre en pratique React Native et Expo
- Implémenter une authentification avec avec **React createContext**
- Gérer la navigation entre plusieurs écrans
- Intégrer une carte interactive
- Accéder à la galerie photo et à la caméra de l'appareil
- Reproduire une application mobile connue avec une architecture claire

---

## 📄 License

Ce projet est fourni à des fins éducatives. Il n’est pas destiné à un usage commercial.

---

## 📡 Contact

- Julien Bouchez : julienbouchez@icloud.com
- Profile GitHub : [@JulienBCHZ](https://github.com/julienb84)
- Profile LinkedIn : [@JulienBouchez](https://www.linkedin.com/in/julien-bouchez-developer/)
