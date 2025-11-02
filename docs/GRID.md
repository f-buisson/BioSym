# BioSym GRIDs
**GRIDs = the networks that connect the modules.**  
Without GRIDs, you just have many modules that don’t communicate.

---

## 1. General Principle

A GRID is:
- a **theme** (water, energy, agriculture, etc.),
- a **main resource** that circulates,
- a **list of required modules**,
- a **list of optional modules**,
- and a **logic of orchestration**.

A GRID can operate independently (e.g., a farm’s WaterGrid)  
or be connected to others (WaterGrid ↔ EnergyGrid ↔ AgroGrid).

---

## 2. Core GRIDs

### 2.1 WaterGrid
- **Mission:** capture, store, treat, and distribute water.  
- **Required modules:**  
  - P (pumping)  
  - S (water storage = tank)  
  - F (filtration)  
  - R (regulation: valves, flow control)  
  - Sense (water level)  
- **Optional modules:** desalination, rainwater harvesting, UV treatment.  
- **Typical workflow:**  
  1. energy available → P pumps to elevated tank  
  2. when tank full → switch to secondary storage  
  3. when potable water requested → pass through F  
  4. for irrigation → divert to soil network

---

### 2.2 EnergyGrid
- **Mission:** circulate electricity from sources to storage and uses.  
- **Required modules:**  
  - E (production)  
  - S (batteries / gravity storage)  
  - R (priorities: essential vs. nonessential loads)  
  - Sense (voltage, current)  
- **Optional modules:** Cp (compressed air), Bio (biogas generator), Act (auto load shedding)  
- **Typical workflow:**  
  - surplus → storage  
  - deficit → discharge  
  - overload → cut noncritical loads

---

### 2.3 DataGrid
- **Mission:** circulate information, not water or electricity.  
- **Required modules:** Sense, Act, orchestrator  
- **Role:** without DataGrid, no AI, no automation.

---

## 3. 3 Concrete Examples

### Example A – “Autonomous Farm (Water + Energy)”
- **Context:** small farm, well, solar panels, vegetable garden.  
- **GRIDs used:** WaterGrid + EnergyGrid + AgroGrid  
- **Flow:**  
  1. EnergyGrid detects sunlight → powers P  
  2. WaterGrid pumps water → fills tank  
  3. AgroGrid checks soil humidity → opens irrigation for 15 min  
  4. If battery full → EnergyGrid authorizes WaterGrid to fill a pond (light EcoGrid)

→ This example illustrates the “useful surplus”.

---

### Example B – “Arid Coast”
- **Context:** coastal village with no freshwater.  
- **GRIDs used:** DesalGrid + WaterGrid + EnergyGrid  
- **Key modules:** P (seawater pump), F (desalination), S (freshwater tank)  
- **Flow:**  
  1. EnergyGrid has surplus (strong wind)  
  2. It authorizes DesalGrid to run (desalination)  
  3. Freshwater goes to WaterGrid  
  4. WaterGrid can send to AgroGrid (artificial oasis)

---

### Example C – “Humanitarian Camp”
- **Context:** no network, basic needs, few technicians.  
- **GRIDs used:** WaterGrid + LightingGrid + WasteGrid  
- **Key modules:** P (pump), F (filter), E (PV), S (battery), R (priorities)  
- **Flow:**  
  - daytime: priority to potable water  
  - nighttime: priority to lighting  
  - if stock low: human message “need 1000L tank”

---

## 4. 20 Possible GRIDs

| GRID Name        | Main Mission                                           | Key Modules                                   |
|------------------|--------------------------------------------------------|-----------------------------------------------|
| WaterGrid        | water capture, storage, treatment                      | P, F, S, R, Sense                             |
| EnergyGrid       | electricity flow, storage, priorities                  | E, S, R, Sense                                |
| AgroGrid         | irrigation, nutrients, greenhouses                     | WaterGrid, soil Sense, R, optionally Bio      |
| DesalGrid        | desalination in coastal zones                          | P (seawater), F (desal), S (freshwater), E    |
| EcoGrid          | support fauna/flora (water points, misting)            | P, S water, R, weather Sense                  |
| HabitatGrid      | home-scale autonomy                                    | EnergyGrid, WaterGrid, R                      |
| WasteGrid        | waste recovery + biogas                                | Bio, WaterGrid, R                             |
| BiogasGrid       | renewable gas network                                  | Bio, R, safety Sense                          |
| ThermalGrid      | heat / solar hot water                                 | solar collectors, S thermal, P, R             |
| MobilityGrid     | EV / bike / local transport charging                   | E, S, R, Sense                                |
| AquacultureGrid  | aquatic basin management                               | P, aeration (Cp), O₂ Sense, R                 |
| GreenhouseGrid   | greenhouse regulation                                  | Sense, Act, P (misting), ThermalGrid          |
| ForestGrid       | fire prevention + occasional watering                  | smoke Sense, P, S water, R                    |
| MarineGrid       | sea energy + water management                          | E (wave/tide), DesalGrid, S                   |
| UrbanGrid        | autonomous neighborhood                                | WaterGrid, EnergyGrid, WasteGrid, MobilityGrid|
| MicroGrid        | shared mini electrical network                         | E, S, R, Sense                                |
| LightingGrid     | autonomous shared lighting                             | E, S, R, light Sense                          |
| CommunicationGrid| off-grid connectivity                                  | E, S, Sense, Act (relay)                      |
| ResilienceGrid   | crisis-response services                               | S (large), P, backup E, R                     |
| NutrientGrid     | liquid fertilizer distribution                         | Bio (digestate), WaterGrid, R                 |
| HealthGrid       | water + energy for healthcare post                     | WaterGrid, EnergyGrid, F, R                   |

---

## 5. GRID Orchestration

A GRID should always answer these 4 questions:

1. **What resource am I circulating?** (water, energy, data, nutrients, etc.)  
2. **Who is allowed to consume it?** (priorities)  
3. **When do I activate the modules?** (based on available energy)  
4. **What if I can’t fulfill the task?** → *human request*

That last point is what makes BioSym realistic:  
👉 when the technology can’t do it → it **asks** (platform, GitHub, donation, local human).

---

# GRIDs BioSym
**Les GRIDs = les réseaux qui relient les modules.**  
Sans GRID, tu as juste plein de modules qui ne se parlent pas.

---

## 1. Principe général

Un GRID, c’est :
- un **thème** (eau, énergie, agriculture…),
- une **ressource principale** qui circule,
- une **liste de modules obligatoires**,
- une **liste de modules optionnels**,
- et une **logique d’orchestration**.

Un GRID peut vivre tout seul (ex : WaterGrid d’une ferme),  
ou être connecté à d’autres GRIDs (WaterGrid ↔ EnergyGrid ↔ AgroGrid).

---

## 2. GRIDs de base

### 2.1 WaterGrid
- **Mission :** capter, stocker, traiter et distribuer de l’eau.
- **Modules requis :**  
  - P (pompage)  
  - S (stockage eau = réservoir)  
  - F (filtration)  
  - R (régulation : ouvrants, vannes)  
  - Sense (niveau d’eau)
- **Modules optionnels :** désalinisation, récupération d’eau de pluie, traitement UV.
- **Fonctionnement type :**
  1. énergie dispo → P pompe vers réservoir haut  
  2. quand réservoir plein → bascule vers stockage secondaire  
  3. quand demande eau potable → passage par F  
  4. quand irrigation → dérivation vers réseau sol

---

### 2.2 EnergyGrid
- **Mission :** faire circuler l’électricité produite par les sources vers les stockages et les usages.
- **Modules requis :**  
  - E (production)  
  - S (batteries / gravité)  
  - R (priorités : charges essentielles vs non essentielles)  
  - Sense (tension, courant)
- **Modules optionnels :** Cp (air comprimé), Bio (générateur biogaz), Act (délestage auto)
- **Fonctionnement type :**
  - surplus → stockage  
  - déficit → déstockage  
  - surcharge → couper charges non critiques

---

### 2.3 DataGrid
- **Mission :** faire circuler les infos, pas l’eau ni l’électricité.
- **Modules requis :** Sense, Act, orchestrateur
- **Rôle :** sans DataGrid, pas d’IA, pas d’automatisation.

---

## 3. 3 exemples concrets

### Exemple A – “Ferme autonome eau + énergie”
- **Contexte :** petite ferme, puits, panneaux solaires, potager.
- **GRIDs utilisés :** WaterGrid + EnergyGrid + AgroGrid
- **Chaînage :**
  1. EnergyGrid voit qu’il y a du soleil → alimente P
  2. WaterGrid remonte l’eau → remplit réservoir
  3. AgroGrid regarde humidité sol → ouvre irrigation 15 min
  4. Si batterie pleine → EnergyGrid autorise WaterGrid à remplir une mare (EcoGrid light)

→ Cet exemple montre le “surplus utile”.

---

### Exemple B – “Côte aride”
- **Contexte :** village côtier sans eau douce.
- **GRIDs utilisés :** DesalGrid + WaterGrid + EnergyGrid
- **Modules clés :** P (pompe eau de mer), F (désal), S (réservoir eau douce)
- **Chaînage :**
  1. EnergyGrid a surplus (vent fort)  
  2. Il autorise DesalGrid à tourner (désalinisation)  
  3. L’eau douce va dans WaterGrid  
  4. WaterGrid peut envoyer vers AgroGrid (oasis artificielle)

---

### Exemple C – “Camp humanitaire”
- **Contexte :** pas de réseau, besoins basiques, pas beaucoup de techniciens
- **GRIDs utilisés :** WaterGrid + LightingGrid + WasteGrid
- **Modules clés :** P (pompe), F (filtre), E (PV), S (batterie), R (priorités)
- **Chaînage :**
  - le jour : priorité à l’eau potable  
  - le soir : priorité à l’éclairage  
  - si stock bas : message humain “besoin d’une cuve 1000L”

---

## 4. 20 GRIDs imaginables

| Nom du GRID     | Mission principale                                      | Modules principaux                              |
|-----------------|---------------------------------------------------------|-------------------------------------------------|
| WaterGrid       | eau, stockage, traitement                               | P, F, S, R, Sense                               |
| EnergyGrid      | électricité, stockage, priorités                        | E, S, R, Sense                                  |
| AgroGrid        | irrigation, nutriments, serres                          | WaterGrid, Sense sol, R, éventuellement Bio     |
| DesalGrid       | désaliniser en zone côtière                             | P (eau mer), F (désal), S (eau fraîche), E      |
| EcoGrid         | soutien faune/flore (points d’eau, brumisateurs)        | P, S eau, R, Sense météo                        |
| HabitatGrid     | autonomie d’une maison                                  | EnergyGrid, WaterGrid, R                        |
| WasteGrid       | valorisation déchets + biogaz                           | Bio, WaterGrid, R                               |
| BiogasGrid      | réseau de gaz renouvelable                              | Bio, R, Sense sécurité                          |
| ThermalGrid     | chaleur / eau chaude solaire                            | capteurs solaires, S thermique, P, R            |
| MobilityGrid    | recharge VE, vélo, transports locaux                    | E, S, R, Sense                                  |
| AquacultureGrid | gestion bassin aquatique                                | P, aération (Cp), Sense O₂, R                   |
| GreenhouseGrid  | régulation serre                                        | Sense, Act, P (brumisation), ThermalGrid        |
| ForestGrid      | prévention incendies + arrosage ponctuel                | Sense fumée, P, S eau, R                        |
| MarineGrid      | énergie de la mer + eau                                 | E (houle/marée), DesalGrid, S                   |
| UrbanGrid       | quartier autonome                                       | WaterGrid, EnergyGrid, WasteGrid, MobilityGrid  |
| MicroGrid       | mini-réseau électrique partagé                          | E, S, R, Sense                                  |
| LightingGrid    | éclairage autonome partagé                              | E, S, R, Sense luminosité                       |
| CommunicationGrid | connectivité off-grid                                 | E, S, Sense, Act (relais)                       |
| ResilienceGrid  | services en cas de crise                                | S (gros), P, E secours, R                       |
| NutrientGrid    | distribution d’engrais liquide                          | Bio (digestat), WaterGrid, R                    |
| HealthGrid      | eau + énergie pour poste de soins                       | WaterGrid, EnergyGrid, F, R                     |

---

## 5. Orchestration d’un GRID

Un GRID doit toujours répondre à ces 4 questions :

1. **Quelle ressource je fais circuler ?** (eau, énergie, données, nutriments…)  
2. **Qui a le droit de la consommer ?** (priorités)  
3. **Quand je lance les modules ?** (en fonction de l’énergie dispo)  
4. **Que faire si je n’y arrive pas ?** → *demande humaine*

C’est ce dernier point qui rend BioSym réaliste :  
👉 quand la techno ne peut pas → elle **demande** (plateforme, GitHub, don, humain local).
