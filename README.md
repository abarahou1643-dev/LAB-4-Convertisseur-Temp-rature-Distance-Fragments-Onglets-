# ConverterTabsJava - Application de Conversion

##  Table des Matières

- [ ConverterTabsJava - Application de Conversion](#️-convertertabsjava---application-de-conversion)
  - [ Table des Matières](#-table-des-matières)
  - [ Fonctionnalités](#-fonctionnalités)
  - [ Technologies Utilisées](#️-technologies-utilisées)
  - [ Structure du Projet](#-structure-du-projet)
  - [ Installation](#️-installation)
  - [ Utilisation](#-utilisation)
  - [Conversion Température](#conversion-température)
  - [Conversion Distance](#conversion-distance)
  - [Sortie de l'Application](#sortie-de-lapplication)
  - [Formules de Conversion](#-formules-de-conversion)
  - [Dépendances](#-dépendances)
  - [Développement](#-développement)
  - [Captures d'Écran](#-captures-décran)
 

## Téléchargement##
**APK de l'Application**
**Téléchargez l'APK directement pour l'installer sur votre appareil Android :**
 **📲 Télécharger l'APK (https://drive.google.com/file/d/16dK4uW96vqF1y4Ehyzg2CuUUQwnRSM1I/view?usp=sharing)
 
##  Fonctionnalités

| Fonctionnalité | Description |
|---------------|-------------|
| **Conversion Température** | Conversion bidirectionnelle Celsius ↔ Fahrenheit |
| **Conversion Distance** | Conversion bidirectionnelle Kilomètres ↔ Miles |
| **Interface à Onglets** | Navigation intuitive entre les différentes conversions |
| **Menu Quitter** | Option de sortie dans le menu de l'application |
| **Confirmation de Sortie** | Boîte de dialogue de confirmation lors de l'appui sur retour |
| **Material Design** | Interface moderne et conforme aux guidelines Material Design |

## Technologies Utilisées

| Composant | Technologie |
|-----------|-------------|
| **Langage** | Java |
| **SDK Minimum** | API 24 (Android 7.0) |
| **Architecture** | Fragments + ViewPager2 |
| **UI Components** | TabLayout, AlertDialog, RadioGroup |
| **Build Tool** | Gradle |

## Structure du Projet

```
ConverterTabsJava/
├── app/
│   └── src/main/
│       ├── java/com/example/convertertabsjava/
│       │   ├── MainActivity.java          # Activité principale
│       │   ├── ViewPagerAdapter.java      # Adapteur pour les onglets
│       │   ├── TempFragment.java          # Fragment température
│       │   └── DistanceFragment.java      # Fragment distance
│       └── res/
│           ├── layout/
│           │   ├── activity_main.xml      # Layout principal
│           │   ├── fragment_temp.xml      # Layout température
│           │   └── fragment_distance.xml  # Layout distance
│           ├── menu/
│           │   └── main_menu.xml          # Menu de l'application
│           └── values/
│               ├── strings.xml            # Chaînes de caractères
│               ├── colors.xml             # Couleurs
│               └── themes.xml             # Thèmes
└── build.gradle.kts                       # Configuration Gradle
```

## Installation

### Prérequis
- Android Studio (version récente)
- SDK Android API 24+
- Emulateur Android ou appareil physique

### Étapes d'installation

1. **Cloner le projet**
   ```bash
   git clone https://github.com/votre-username/ConverterTabsJava.git
   ```

2. **Ouvrir avec Android Studio**
   - File → Open → Sélectionner le dossier du projet

3. **Synchroniser les dépendances**
   - Cliquer sur "Sync Now" lorsque demandé

4. **Compiler et exécuter**
   -  Run → Select Device → Choisir un émulateur/appareil

## Utilisation

### Conversion Température
1. **Sélectionner le sens de conversion**
   - "C → F" : Celsius vers Fahrenheit
   - "F → C" : Fahrenheit vers Celsius

2. **Saisir la valeur**
   - Entrer la valeur numérique dans le champ

3. **Calculer**
   - Cliquer sur le bouton "Calculer"
   - Le résultat s'affiche automatiquement

**Exemple** : 25°C → 77.00°F

### Conversion Distance
1. **Sélectionner le sens de conversion**
   - "Km → Miles" : Kilomètres vers Miles
   - "Miles → Km" : Miles vers Kilomètres

2. **Saisir la valeur**
   - Entrer la valeur numérique dans le champ

3. **Calculer**
   - Cliquer sur le bouton "Calculer"

**Exemple** : 10km → 6.21 miles

### Sortie de l'Application
- **Méthode 1** : Menu → "Quitter"
- **Méthode 2** : Bouton retour physique/personnalisé
- **Confirmation** : Boîte de dialogue demande confirmation

## Formules de Conversion

### Température
| Conversion | Formule |
|------------|---------|
| **Celsius → Fahrenheit** | `°F = (1.8 × °C) + 32` |
| **Fahrenheit → Celsius** | `°C = (°F - 32) / 1.8` |

### Distance
| Conversion | Formule |
|------------|---------|
| **Kilomètres → Miles** | `miles = km × 0.6214` |
| **Miles → Kilomètres** | `km = miles / 0.6214` |

## Dépendances

```kotlin
dependencies {
    implementation("androidx.appcompat:appcompat:1.6.1")
    implementation("com.google.android.material:material:1.12.0")
    implementation("androidx.constraintlayout:constraintlayout:2.1.4")
    implementation("androidx.viewpager2:viewpager2:1.0.0")
    
    // Testing
    testImplementation("junit:junit:4.13.2")
    androidTestImplementation("androidx.test.ext:junit:1.1.5")
    androidTestImplementation("androidx.test.espresso:espresso-core:3.5.1")
}
```

## Développement

### Compétences mises en œuvre
-  Fragments et ViewPager2
-  TabLayout avec TabLayoutMediator
-  Gestion des événements utilisateur
-  Dialogues de confirmation Material Design
-  Interface responsive
-  Validation des entrées utilisateur

### Architecture
```
MainActivity
    ├── ViewPagerAdapter
    │   ├── TempFragment
    │   └── DistanceFragment
    ├── TabLayout
    └── ViewPager2
```

## Captures d'Écran



https://github.com/user-attachments/assets/1b8abe46-827d-4792-9a34-dd61b2c9512c




https://github.com/user-attachments/assets/78d21309-f654-4e8c-adf7-46605a9a252c




