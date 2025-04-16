# ESPHome Project for Equip'Care - SupDeVinci

Ce projet ESPHome est conçu pour gérer les fonctionnalités d'**Equip'Care**, un projet développé à SupDeVinci Rennes. Il utilise un ESP32 pour intégrer un capteur ultrasonique, un buzzer, et un clavier matriciel 4x4. 

---

## 📋 Fonctionnalités

- **HC-SR04** : Mesure de distance via capteur ultrasonique.
- **Buzzer** : Génération de sons et mélodies avec le module `rtttl`.
- **Keypad matriciel 4x4** : Collecte de codes PIN et contrôle interactif.

---

## 🛠️ Matériel requis

- **ESP32** (ESP32Dev ou compatible).
- **Capteur ultrasonique HC-SR04**.
- **Buzzer actif 2 pins**.
- **Keypad matriciel 4x4 (8 pins)**.
- Alimentation 5V pour ESP32.

---

## ⚙️ Câblage

### Buzzer (2 pins)
- **+ (positif)** → GPIO27
- **- (négatif)** → GND

### Keypad Matriciel 4x4
- **Row 1** → GPIO18
- **Row 2** → GPIO5
- **Row 3** → GPIO17
- **Row 4** → GPIO16
- **Column 1** → GPIO4
- **Column 2** → GPIO0
- **Column 3** → GPIO2
- **Column 4** → GPIO15



---

## 🔌 Connexion à ESPHome

Pour configurer et déployer ce projet, utilisez les étapes suivantes :

1. Ajoutez votre ESP32 à **ESPHome** via l'application mobile ou l'interface web.
2. Téléchargez ce projet dans votre dépôt local et modifiez les secrets Wi-Fi dans le fichier `secrets.yaml`.

---

## 🌐 Modules ESPHome requis

Assurez-vous que votre installation ESPHome supporte les modules suivants :
- `matrix_keypad`
- `rtttl`
- `ultrasonic`

Vous pouvez installer ces modules via ESPHome si nécessaire.

---

## 📁 Fichiers importants

- **`domocare-esp.yaml`** : Configuration principale du projet ESPHome.
- **`secrets.yaml`** : Contient les informations Wi-Fi (non inclus dans le dépôt pour des raisons de sécurité voir secrets.yaml.exemple).
- **`.gitignore`** : Empêche de pousser les fichiers sensibles comme `secrets.yaml`.
