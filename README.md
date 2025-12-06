# README - Projet Web Mapping 2025

## Visualisation Multi-Couches - Données Géospatiales

### Description du Projet
Ce projet implémente une application web de visualisation interactive de données géospatiales (NDVI, RGB, NDWI) exportées depuis GeoServer. L'application permet une exploration dynamique des données avec contrôle individuel des couches et ajustement en temps réel.

---

## Objectifs Réalisés

### Exercice 3 : Visualisation d'images drones et satellites via GeoServer
1. Publication des données : Export et hébergement des couches NDVI, RGB et NDWI
2. Styles appliqués : Visualisation avec légendes appropriées pour chaque indice
3. Interface interactive : Carte Leaflet avec contrôles de couches
4. Analyse comparative : Comparaison des différentes méthodes de visualisation

---

## Technologies Utilisées

| Technologie | Rôle | Version |
|------------|------|---------|
| Leaflet | Bibliothèque cartographique | 1.9.4 |
| GeoServer | Serveur de données géospatiales | 2.23.x |
| HTML5/CSS3 | Interface utilisateur | - |
| JavaScript | Logique interactive | ES6 |
| PNG/GeoTIFF | Format des données exportées | - |

---

## Structure du Projet

```
projet-web-mapping/
│
├── index.html              # Interface principale
├── NDVI.png                # Image NDVI exportée
├── RGB.png                 # Image RGB exportée  
├── NDWI.png                # Image NDWI exportée
│
├── docs/                   # Documentation supplémentaire
│   ├── rapport-technique.pdf
│   └ captures-ecran/
│
└── README.md              # Ce fichier
```

---

## Installation et Utilisation

### Option 1 : Utilisation Directe (GitHub Pages)
1. Rendez-vous sur : https://[votre-username].github.io/[nom-du-repo]/
2. L'interface se charge automatiquement

### Option 2 : Exécution Locale
1. Téléchargez les fichiers du projet
2. Ouvrez index.html dans un navigateur web
3. Assurez-vous que les images (NDVI.png, RGB.png, NDWI.png) sont dans le même dossier

---

## Fonctionnalités de l'Interface

### Contrôles Disponibles
- Activation/Désactivation des couches NDVI, RGB et NDWI
- Ajustement d'opacité pour chaque couche (0% à 100%)
- Boutons rapides : "Afficher Tout" / "Masquer Tout"
- Légende dynamique qui s'adapte à la couche active
- Coordonnées en temps réel au survol de la carte
- Informations détaillées au clic sur la carte

### Navigation Carte
- Zoom avec molette de souris
- Déplacement par glisser-déposer
- Recentrage automatique sur la zone d'étude

---

## Couches Disponibles

### NDVI (Normalized Difference Vegetation Index)
- Objectif : Évaluer la santé et la densité de la végétation
- Plage de valeurs : -1 à 1
- Légende :
  - -1 → Valeurs très faibles
  - 0 → Sol nu
  - 0.2 → Végétation clairsemée
  - 0.5 → Végétation modérée
  - 1 → Végétation dense

### RGB (Composition Colorée Naturelle)
- Objectif : Visualisation en couleurs naturelles
- Bandes utilisées : Rouge, Vert, Bleu
- Résolution : 30 mètres/pixel

### NDWI (Normalized Difference Water Index)
- Objectif : Détection de l'eau et de l'humidité
- Plage de valeurs : -1 à 1
- Application : Identification des plans d'eau et zones humides

---

## Configuration Technique

### Systèmes de Coordonnées
- Données sources : UTM Zone 32N (EPSG:32632)
- Affichage web : Web Mercator (EPSG:3857)
- Reprojection : Automatique par GeoServer/Leaflet

### Performances
- Chargement optimisé des images PNG
- Interface responsive
- Compatibilité multi-navigateurs

---

## Analyse et Résultats

### Points Forts
1. Interface intuitive : Navigation facile même pour non-experts
2. Performance : Chargement rapide des couches
3. Interactivité : Contrôles en temps réel
4. Compatibilité : Fonctionne sur tous les navigateurs modernes

### Limitations
1. Données statiques : Les images doivent être régénérées pour les mises à jour
2. Géoréférencement : Positionnement manuel nécessaire pour les PNG
3. Volume : Les images haute résolution peuvent être volumineuses

---

## Recommandations pour Amélioration

### Court Terme
- Ajout d'un sélecteur de date/temps pour données temporelles
- Implémentation de l'export d'images depuis l'interface
- Ajout de couches de contexte supplémentaires

### Moyen Terme
- Migration vers Cloud Optimized GeoTIFF (COG)
- Intégration avec API GeoServer en direct
- Ajout de calculs d'indices en temps réel

---

## Contributeurs

- Étudiant : [Votre Nom]
- Encadrant : [Nom de l'Encadrant]
- Institution : IAV Hassan II
- Date : 2025

---

## Références

1. Documentation Leaflet : https://leafletjs.com/
2. Documentation GeoServer : https://geoserver.org/
3. Indices Spectraux : NASA Earth Observatory
4. Tutoriels Web Mapping : OpenGeoEdu

---

## Licence

Ce projet est développé dans le cadre académique de l'IAV Hassan II.
Les données sont fournies à titre éducatif et de démonstration.

---

## Liens Utiles

- Application en ligne : [Lien GitHub Pages]
- Code source : [Lien vers le repository]
- Rapport complet : [Lien vers le rapport PDF]

---

Dernière mise à jour : Mars 2025  
Projet réalisé dans le cadre du module Web Mapping - IAV Hassan II
