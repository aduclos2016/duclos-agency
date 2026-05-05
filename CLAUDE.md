# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

Site web vitrine de Duclos Agency — expérience interactive 3D destinée à présenter les services de l'agence avec des animations et une navigation immersive.

## Stack envisagée

Ce projet est orienté vers des sites web dynamiques 3D. Les technologies cibles typiques pour ce type de projet sont :

- **Three.js** ou **R3F (React Three Fiber)** pour le rendu 3D WebGL
- **GSAP** pour les animations et transitions
- **Vite** comme bundler
- **React** ou JavaScript vanilla selon la complexité

> Mettre à jour cette section dès que la stack est fixée.

## Commandes de développement

> À compléter une fois le projet initialisé (ex: `npm create vite@latest`, `npm install three`, etc.)

```bash
# Exemple (à adapter)
npm install        # Installer les dépendances
npm run dev        # Lancer le serveur de développement
npm run build      # Build de production
npm run preview    # Prévisualiser le build
```

## Architecture

> À documenter au fur et à mesure. Décrire ici :
> - L'organisation des scènes 3D (ex: une scène par section de page)
> - La gestion du scroll (ex: ScrollTrigger + caméra animée)
> - Les assets 3D (modèles `.glb`/`.gltf`, textures, shaders GLSL)
> - L'état global si applicable (Zustand, Context, etc.)

## Conventions spécifiques au projet

- Les shaders GLSL personnalisés vont dans `src/shaders/`
- Les modèles 3D et assets vont dans `public/models/`
- Éviter les imports volumineux inutiles de Three.js — utiliser les imports ciblés (`import { Mesh } from 'three'`)
