# 📡 Antenne Loop Omnidirectionnelle Active 1-30 MHz

Projet KiCad 9 complet pour une antenne loop double boucle amplifiée avec accord varicap à distance.

## 📋 Contenu du projet

### PCB 1 : Boîtier de Commande (100mm × 80mm)
- **Fichier** : `pcb/pcb1_control/control_box.kicad_sch`
- **Fonction** : Injection DC 12V + Signal varicap 0-12V
- **Composants** : 7 (Fusible, Potentiomètre, Résistance, Condensateur, Diode, Connecteurs)

### PCB 2 : Boîtier Amplificateur (150mm × 120mm)
- **Fichier** : `pcb/pcb2_amplifier/amplifier_box.kicad_sch`
- **Fonction** : Amplification RF (BF998 FET + 2N3904 Buffer)
- **Gain** : 20-25 dB @ 10 MHz
- **Composants** : 20+ (Transistors, Résistances, Condensateurs, Inductances, Diodes)

### PCB 3 : Hybrid Coupler 90° (100mm × 100mm)
- **Fichier** : `pcb/pcb3_coupler/hybrid_coupler.kicad_sch`
- **Fonction** : Combinaison des deux boucles (N-S et E-O)
- **Déphasage** : 90° pour omnidirectionnalité
- **Composants** : 14 (Résistances, Condensateurs, Diodes, Connecteurs)

## 🎯 Spécifications

| Paramètre | Valeur |
|---|---|
| Fréquence | 1-30 MHz |
| Gain | 20-25 dB |
| Figure de bruit | < 3 dB @ 1 MHz |
| Directivité | Omnidirectionnelle ±3 dB |
| Alimentation | 12V DC, 80-100 mA |
| Accord | Varicap 0-12V (manuel à distance) |
| Câble | RG58 50Ω (max 50m) |
| Impédance sortie | 50Ω |

## 🔧 Logiciels requis

- **KiCad 9.0.7+** (Linux, macOS, Windows)
- **Ubuntu 24.04** (testé)
- **Git** (pour cloner le dépôt)

## 📥 Installation

### Cloner le dépôt avec SSH

```bash
git clone git@github.com:VOTRE_USERNAME/antenne-loop-kicad.git
cd antenne-loop-kicad
