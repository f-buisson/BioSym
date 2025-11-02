# BioSym Modules
Each module = 1 clear function.  
They are then assembled together within the GRIDs.

---

## List of Core Modules

1. **E** – Energy Module  
2. **P** – Pumping Module  
3. **F** – Filtration / Water Treatment Module  
4. **S** – Storage Module (electric or gravity)  
5. **Cp** – Compression / Compressed Air Module  
6. **R** – Regulation Module (valves, priorities, flow)  
7. **Sense** – Sensor / Data Module  
8. **Act** – Actuator Module (open, close, start)  
9. **Bio** – Biogas / Organic Recovery Module  
10. **Aux** – Human Backup Module (pedal, crank, emergency generator)

---

## 1. Energy Module (E)

**Purpose:** provide base electricity to the system.  
**Possible inputs:**
- solar PV panel,  
- small wind turbine,  
- micro-hydro source (stream),  
- optionally biogas → generator.

**Outputs:**
- 12/24/48 V DC (depending on your chosen standard),  
- optionally 230 V via inverter.

**Role in BioSym:**
- powers the pump,  
- powers sensors,  
- charges storage,  
- top priority (no energy → no system).

**Notes:**
- you can plan 2 levels:  
  - E-Lite: just PV + regulator  
  - E-Full: PV + wind + battery + inverter

---

## 2. Pumping Module (P)

**Purpose:** move water.  
**Power sources:** Energy Module (E) or direct energy (wind pump, water wheel).  
**Outputs:** water directed to:  
- elevated tank (gravity storage),  
- irrigation network,  
- desalination,  
- treatment.

**Possible types:**
- DC solar pump  
- membrane pump  
- low-tech volumetric pump

**Role in BioSym:**  
It’s what makes energy surpluses useful (when there’s too much sun → we pump).

---

## 3. Filtration / Treatment Module (F)

**Purpose:** make water usable.  
**Inputs:** raw water (well, river, rain, sea for desalination).  
**Energy:** very low (UV, circulation pump) or thermal (solar distillation).  
**Outputs:** potable or irrigation-ready water.

**Sub-types:**
- F-lite: gravity filter + solar UV  
- F-desal: reverse osmosis → requires a P module upstream  
- F-solar: solar distillation (slow but autonomous)

**Role:** essential for WaterGrid.

---

## 4. Storage Module (S)

**Purpose:** smooth variations.  
**Two main families:**
1. **S-elec:** batteries, supercaps  
2. **S-gravity:** elevated water, lifted mass  
3. (**optional**) S-thermal: solar hot water

**Input:** energy or water  
**Output:** energy or pressurized water  
**Role:** allows BioSym to run at night / without wind.

---

## 5. Compression Module (Cp)

**Purpose:** store surplus energy as compressed air.  
**Input:** excess energy (E)  
**Output:** compressed air (for tools, turbines, pond aeration)

**Advantages:**
- no chemistry,  
- can be DIY,  
- great combo with wind (wind → direct compression)

**Limits:**
- average efficiency, best for sites with frequent surpluses.

---

## 6. Regulation Module (R)

**Purpose:** decide what to let through.  
**Examples:**
- solenoid valve on irrigation network  
- divert water to storage when the main tank is full  
- shed electrical load

**Inputs:** commands from AI / simple rules  
**Outputs:** open/close, ON/OFF, circuit choice

**Role:** it’s the system’s “vascular network”.

---

## 7. Sensor / Data Module (Sense)

**Purpose:** know what’s happening.  
**Typical sensors:**
- water tank level  
- battery voltage  
- flow rate  
- soil humidity  
- weather (light, wind)

**Output:** data to DataGrid / orchestrator

---

## 8. Actuator Module (Act)

**Purpose:** move what regulation decides.  
- stepper motors (open greenhouse window)  
- relays (start a pump)  
- servos (orient a solar panel)

---

## 9. Biogas Module (Bio)

**Purpose:** turn waste into energy + fertilizer  
**Input:** organic waste, heat  
**Outputs:** biogas + digestate  
**Use:** backup energy + agricultural loop (see AgroGrid)

---

## 10. Human Backup Module (Aux)

**Purpose:** allow a human to “save” the system when there’s no sun/wind  
**Examples:** pedal generator, foot pump, crank  
**Role:** ensure resilience

---

## Quick Summary

| Name  | Purpose                     | Essential?      |
|--------|-----------------------------|-----------------|
| E      | produce energy              | ⭐️ yes          |
| P      | move water                  | ⭐️ yes (if water) |
| F      | make water clean            | ⭐️ yes (if water) |
| S      | buffer / smooth operations  | ⭐️ yes          |
| R      | orchestrate flows           | ⭐️ yes          |
| Sense  | measure                     | useful          |
| Bio    | close organic loops         | optional        |
| Cp     | alternative storage         | optional        |

You can create a **BioSym-min** version with:  
**E + P + F + S + R + Sense**

---

# Modules BioSym
Chaque module = 1 fonction claire.  
On les assemble ensuite dans les GRIDs.

---

## Liste des modules de base

1. **E** – Module Énergie  
2. **P** – Module Pompage  
3. **F** – Module Filtration / Traitement d’eau  
4. **S** – Module Stockage (élec ou gravité)  
5. **Cp** – Module Compression / air comprimé  
6. **R** – Module Régulation (vannes, priorités, débit)  
7. **Sense** – Module Capteurs / Data  
8. **Act** – Module Actionneurs (ouvrir, fermer, démarrer)  
9. **Bio** – Module Biogaz / valorisation organique  
10. **Aux** – Module d’appoint humain (pédale, manivelle, groupe de secours)

---

## 1. Module Énergie (E)

**But :** fournir l’électricité de base au système.  
**Entrées possibles :**
- panneau solaire PV,
- petite éolienne,
- micro-hydro (cours d’eau),
- éventuellement biogaz → groupe électrogène.

**Sorties :**
- 12/24/48 V DC (selon ce que tu veux standardiser),
- éventuellement 230 V via onduleur.

**Rôle dans BioSym :**
- alimente la pompe,
- alimente les capteurs,
- charge le stockage,
- sert de priorité 1 (sans énergie → pas de système).

**Remarques :**
- tu peux prévoir 2 niveaux :  
  - E-Lite : juste PV + régulateur  
  - E-Full : PV + éolien + batterie + onduleur

---

## 2. Module Pompage (P)

**But :** déplacer de l’eau.  
**Sources d’énergie :** module Énergie (E) ou énergie directe (éolienne à pompe, roue à aubes).  
**Sorties :** eau vers :  
- réservoir haut (stockage gravitaire),  
- réseau d’irrigation,  
- désalinisation,  
- traitement.

**Types possibles :**
- pompe DC solaire
- pompe à membrane
- pompe volumétrique low-tech

**Rôle dans BioSym :**
- c’est lui qui rend utiles les surplus d’énergie (quand il y a trop de soleil → on pompe)

---

## 3. Module Filtration / Traitement (F)

**But :** rendre l’eau utilisable.  
**Entrées :** eau brute (puits, rivière, pluie, mer si désalinisation).  
**Énergie :** très faible (UV, pompe de circulation) ou thermique (distillation solaire).  
**Sorties :** eau potable / eau d’irrigation propre.

**Sous-types :**
- F-lite : filtre gravité + UV solaire  
- F-desal : osmose inverse → besoin d’une pompe P en amont  
- F-solaire : distillation solaire (lent mais autonome)

**Rôle :** indispensable pour WaterGrid.

---

## 4. Module Stockage (S)

**But :** lisser les variations.  
**Deux grandes familles :**
1. **S-élec** : batteries, supercaps
2. **S-gravité** : eau en hauteur, masse hissée
3. (**optionnel**) S-thermique : eau chaude solaire

**Entrée :** énergie ou eau  
**Sortie :** énergie ou eau sous pression  
**Rôle :** permet à BioSym de continuer à fonctionner la nuit / sans vent.

---

## 5. Module Compression (Cp)

**But :** stocker un surplus sous forme d’air comprimé.  
**Entrée :** énergie excédentaire (E)  
**Sortie :** air comprimé (pour outils, pour turbinage, pour aération bassin)

**Avantages :**
- pas de chimie,
- peut être bricolé,
- bon en combiné avec éolien (vent → compression directe)

**Limites :**
- rendement moyen, à réserver aux sites avec excédents fréquents.

---

## 6. Module Régulation (R)

**But :** décider quoi laisser passer.  
**Exemples :**
- électrovanne sur réseau d’irrigation
- dérivation d’eau vers stockage quand réservoir principal plein
- délestage d’une charge électrique

**Entrées :** consignes de l’IA / règles simples  
**Sorties :** ouverture/fermeture, ON/OFF, choix de circuit

**Rôle :** c’est le “système vasculaire” du truc.

---

## 7. Module Capteurs / Data (Sense)

**But :** savoir ce qu’il se passe.  
**Capteurs typiques :**
- niveau d’eau dans réservoir
- tension batterie
- débit
- humidité sol
- météo (luminosité, vent)

**Sortie :** données vers DataGrid / orchestrateur

---

## 8. Module Actionneurs (Act)

**But :** faire bouger ce que la régulation décide.  
- moteurs pas à pas (ouvrir fenêtre serre)
- relais (démarrer une pompe)
- servo (orienter panneau)

---

## 9. Module Biogaz (Bio)

**But :** valoriser les déchets en énergie + fertilisant  
**Entrée :** déchets organiques, chaleur  
**Sorties :** biogaz + digestat  
**Utilité :** énergie de secours + boucle agricole (voir AgroGrid)

---

## 10. Module d’appoint humain (Aux)

**But :** permettre à un humain de “sauver” le système quand pas de soleil/pas de vent  
**Ex :** vélo générateur, pompe à pédale, manivelle  
**Rôle :** assurer la résilience

---

## Synthèse rapide

| Nom   | Sert à…                  | Indispensable ? |
|-------|--------------------------|-----------------|
| E     | produire de l’énergie    | ⭐️ oui          |
| P     | déplacer de l’eau        | ⭐️ oui (si eau) |
| F     | rendre l’eau propre      | ⭐️ oui (si eau) |
| S     | lisser / tamponner       | ⭐️ oui          |
| R     | orchestrer les flux      | ⭐️ oui          |
| Sense | mesurer                  | utile           |
| Bio   | boucler les matières     | optionnel       |
| Cp    | stocker autrement        | optionnel       |

Tu peux donc faire une version **BioSym-min** avec :  
**E + P + F + S + R + Sense**.
