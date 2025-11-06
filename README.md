[![Sponsor](https://img.shields.io/badge/Sponsor-Fabien%20Buisson-6E56CF?style=for-the-badge)](https://github.com/sponsors/f-buisson)

# 🌍 BioSym  
**Symbiotic Modular System for Water, Energy, and Regeneration**

BioSym is a **conceptual open-source project** designed to show how we can **combine existing technologies** (solar, wind, pumping, filtration, storage, sensors, local AI) to create **useful autonomous systems** — pumping water, treating it, storing energy, irrigating, powering greenhouses, desalinating, and more.  

BioSym serves as a **framework** for imagining, documenting, and sharing these combinations.

> 💡 It’s a **project for the future**, not a finished machine.  
> It’s made to be **read, reused, improved, and challenged**.

---

## 🧭 What It Is

- An **architecture** describing how to connect water, energy, and storage modules.  
- A **“GRID” system** (thematic networks) to circulate water, energy, and data.  
- An **orchestration layer** (AI / rules / logic) to decide what to activate, when, and why.  
- An **open-hardware / open-doc project** — anyone can propose their own modules.

---

## 🧩 Global Architecture

BioSym consists of four layers:

1. **Modules**  
   Independent technical building blocks:  
   - P = Pumping  
   - F = Filtration / Potabilization  
   - E = Energy production (PV, wind, hydro, etc.)  
   - S = Storage (batteries, gravity, compressed air)  
   - Cp = Compression  
   - R = Regulation / valves / priority control  
   → See: [`docs/Modules.md`](docs/Modules.md)

2. **Grids (Networks)**  
   These are the “circulations” between modules.  
   - **WaterGrid** → everything related to water  
   - **EnergyGrid** → all things electrical / energetic  
   - **DataGrid** → data, sensors, control signals  
   - + thematic grids (AgriGrid, DesalGrid, EcoGrid, etc.)  
   → See: [`docs/GRID.md`](docs/GRID.md)

3. **Orchestrator (AI or Rules)**  
   - observes sensors  
   - detects surpluses (energy, water)  
   - activates the right modules at the right time  
   - can publish a **“human request”** when something is missing (pipe, tank, larger pump, etc.)

4. **Humans in the Loop**  
   - build the parts the AI cannot  
   - validate critical decisions  
   - adapt the system to the field context

---

## 🎯 Objectives

- Show that we can **achieve a lot with existing technologies** if properly linked.  
- Provide a **documentary base** for other makers / NGOs / engineers.  
- Prepare for a future where **multiple environmental AIs cooperate** (desalinate here, irrigate there, store energy elsewhere).

---

## 🗂 Repository Content

- `README.md` (this file)  
- `docs/Vision.md` → why BioSym exists, philosophy, nature/tech link  
- `docs/Modules.md` → description of each module  
- `docs/GRID.md` → how modules interconnect + 3 examples + 20 imaginative GRIDs  
- `docs/Roadmap.md` → how the project can evolve (no deadlines)

---

## 🛠 How to Contribute

1. Read the vision → [`docs/Vision.md`](docs/Vision.md)  
2. Propose a **new module** (low-tech pump, mini wind turbine, solar filter, etc.)  
3. Or propose a **new GRID** (e.g., “RefugeGrid,” “ForestGrid,” “HumanitarianCampGrid”)  
4. Or make an **orchestration diagram** (who talks to whom, in what order)

The idea: **it doesn’t have to be built to be shared.**  
We document first, prototype later.

---

## 🚧 Roadmap (No Dates)

1. 📄 **“Ideas” Phase** – gather modules, grids, and use cases  
2. 🧪 **“Small Prototypes” Phase** – 1 water module + 1 energy module + 1 logic layer  
3. 🔁 **“Chaining” Phase** – make several modules work together  
4. 🌱 **“Field” Phase** – small autonomous demonstrato

---

### 🫶 Support this project

I release these projects as **open-hardware**, so anyone can study, adapt, and rebuild them freely.  
If you'd like to help the development continue and support new prototypes:  
👉 https://github.com/sponsors/f-buisson  
Even a symbolic contribution helps to:
- fund necessary materials
- develop and test prototypes
- cover software licensing fees (SolidWorks, etc.)

Thank you for your support ✦

---

# 🌍 BioSym
**Système symbiotique modulaire pour l’eau, l’énergie et la régénération**

BioSym est un projet **conceptuel open-source** dont l’objectif est de montrer comment on peut **combiner des technologies déjà existantes** (solaire, éolien, pompage, filtration, stockage, capteurs, petite IA locale) pour créer **des systèmes autonomes utiles** : pomper de l’eau, la traiter, stocker de l’énergie, irriguer, alimenter une serre, désaliniser, etc.

BioSym sert donc de **cadre** pour imaginer, documenter et partager ces combinaisons.

> 💡 C’est un projet d’avenir, pas une machine finie.  
> Il est fait pour être lu, repris, amélioré, challengé.

---

## 🧭 Ce que c’est

- Une **architecture** qui décrit comment relier des modules d’eau, d’énergie et de stockage.
- Un **système de “GRID”** (réseaux thématiques) pour faire circuler eau, énergie et données.
- Une **couche d’orchestration** (IA / règles / logique) pour décider quoi activer, quand et pourquoi.
- Un **projet open-hardware / open-doc** : chacun peut proposer ses propres modules.

---

## 🧩 Architecture globale

BioSym est composé de 4 couches :

1. **Modules**  
   Petites briques techniques indépendantes :  
   - P = pompage  
   - F = filtration / potabilisation  
   - E = production d’énergie (PV, éolien, hydro…)  
   - S = stockage (batteries, gravité, air comprimé)  
   - Cp = compression  
   - R = régulation / vannes / priorités  
   → Voir : [`docs/Modules.md`](docs/Modules.md)

2. **Grids (réseaux)**  
   Ce sont les “circulations” entre modules.  
   - WaterGrid → tout ce qui est eau  
   - EnergyGrid → tout ce qui est électricité / énergie  
   - DataGrid → données, capteurs, commandes  
   - + grilles thématiques (AgriGrid, DesalGrid, EcoGrid, etc.)
   → Voir : [`docs/GRID.md`](docs/GRID.md)

3. **Orchestrateur (IA ou règles)**  
   - observe les capteurs  
   - voit les surplus (énergie, eau)  
   - lance les bons modules au bon moment  
   - peut publier une **“demande humaine”** quand il manque un élément (conduit, réservoir, pompe plus grosse…)

4. **Humains dans la boucle**  
   - fabriquent les pièces que l’IA ne peut pas faire  
   - valident les choix sensibles  
   - adaptent le système au terrain

---

## 🎯 Objectifs

- montrer qu’on peut **faire beaucoup avec des technologies déjà là** si on les enchaîne bien ;
- fournir une **base documentaire** pour d’autres makers / ONG / ingénieurs ;
- préparer un futur où **plusieurs IA environnementales coopèrent** (désaliniser ici, irriguer là-bas, stocker ailleurs).

---

## 🗂 Contenu du dépôt

- `README.md` (ce fichier)
- `docs/Vision.md` → pourquoi BioSym, philosophie, lien nature/techno
- `docs/Modules.md` → description de chaque module
- `docs/GRID.md` → comment on relie les modules + 3 exemples + 20 GRIDs imaginables
- `docs/Roadmap.md` → comment faire évoluer le projet sans dates

---

## 🛠 Comment contribuer

1. Lire la vision → [`docs/Vision.md`](docs/Vision.md)
2. Proposer un **nouveau module** (pompe low-tech, mini-éolienne, filtre solaire…)
3. Ou proposer un **nouveau GRID** (par ex. “RefugeGrid”, “ForestGrid”, “CampHumanitaireGrid”)
4. Ou faire un **schéma d’orchestration** (qui parle à qui ? dans quel ordre ?)

L’idée : **pas besoin que ce soit construit pour être partagé.**  
On documente d’abord, on prototype après.

---

## 🚧 Roadmap (sans dates)

1. 📄 **Phase “idées”** – recenser modules, grilles, cas d’usage  
2. 🧪 **Phase “petits protos”** – 1 module eau + 1 module énergie + 1 logique  
3. 🔁 **Phase “chaînage”** – faire fonctionner plusieurs modules ensemble  
4. 🌱 **Phase “terrain”** – petit démonstrateur autonome (ferme, serre, camp)  
5. 🔗 **Phase “réseau”** – plusieurs BioSym qui échangent

→ Détails : [`docs/Roadmap.md`](docs/Roadmap.md)

---

## ❗️Important

- BioSym **n’est pas** une promesse d’énergie infinie.  
- BioSym **est** une façon d’organiser des technos connues pour faire mieux avec peu.  
- Le projet peut rester **théorique** jusqu’à ce qu’une équipe, un fablab ou une ONG veuille en prototyper une partie.

---

## ✉️ Contact / usage

Si tu reprends ce concept, précise l’origine : **“Concept BioSym inspiré par projet open-source (f-buisson)”**  
Ça permettra aux prochains de remonter à la source.

---

### 🫶 Soutenir ce projet

Je publie ces projets en **open-hardware**, pour que chacun puisse les comprendre, les adapter et les reconstruire librement.  
Si tu souhaites contribuer à leur évolution et à la création de nouveaux prototypes :  
👉 https://github.com/sponsors/f-buisson  
Chaque contribution (même symbolique) permet de :
- financer les matériaux nécessaires
- développer et tester les prototypes
- couvrir les licences logicielles (SolidWorks, etc.)

Merci pour ton soutien ✦
