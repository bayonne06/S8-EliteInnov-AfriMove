# AfriMove — Covoiturage inter-quartiers, Brazzaville

Bienvenue dans votre startup. Ce dépôt est le **squelette** de l'application : un mini-site de 9 pages pour organiser le covoiturage entre habitants des quartiers de Brazzaville. La structure est déjà en place ; **votre équipe complète les fonctions manquantes et construit les pages**.

# Parcours et tâches effectuées par membres 

**Devs Fullstacks**
---------------------
|Nom et prénoms|code- tâches|rôle|adresse mail|
|:--------------|-----------|----|------------|
|NKODIA De Matsika Luc Dalland| FS1 - Accueil | - |lucdalland@gmail.com|
|KEDO Tony Bérenger| FS6 - Dashboard et Confirmation| Lead Dev | berengerkedo@gmail.com|
|HIRWA Jean Baptiste| FS2 - Rechercher | - | contact.jean.dev@gmail.com|
|Mavoungou Bayonne Précieux|FS4,FS3 -Proposer, Trajet | Repo admin| bayonnepre@gmail.com|
|CHANPUISSAT Marlond Lothaire|FS7 - Inscription,Log In|-|chanpuissant@gmail.com|
|MIKOLO Rolvi | FS5 - Mes trajets | - | rolvymikolo@gmail.com|


Vous avez **quelques jours** pour ce projet.


**DATA ANALYSTES**
---------------------

**Zone A**
-----------
|Nom et prénoms|Fonctionnalité d'ensemble| fonction|
|--------------|-------------------------|------|
|AZIDAMA Belvine| Recherche| --//---|

**Zone B**
|Nom et prénoms| Fonctionnalité d'ensemble| fonction|
|--------------|--------------------------|---------|
|MOUSSONI Grâce| Réservation| compter réservation par trajet, vérifier place disponible, calculer taux d'annulation|
|AZIDAMA Belvine| Réservation|filtré réservation par status, historique réservation passager|

**Zone C**
|Nom et prénoms| Fonctionnalité d'ensemble| fonction|
|--------------|--------------------------|---------|
|MOUSSONI Grâce| Statistiques| --//--|


**Zone D**
|Nom et prénoms| Fonctionnalité d'ensemble| fonction|
|--------------|--------------------------|---------|
|AZIDAMA Belvine| Comptes | vérifier téléphone disponible|
|MOUSSONI Grâce| Comptes | trouver compte par téléphone|

## Lancer le projet en local

**1. Démarrer l'API (un seul terminal, à laisser ouvert)**

```bash
cd backend
pip install -r requirements.txt
python app.py
```

L'API tourne sur `http://localhost:5000`. Laissez ce terminal ouvert tout le temps où vous travaillez.

**2. Ouvrir le site**

**Si vous utilisez VS Code, l'extension Live Server fonctionne aussi très bien (clic droit sur le fichier HTML → "Open with Live Server").**

**C'est tout : un seul terminal pour l'API, et vous ouvrez vos pages HTML directement.** Tant que `python app.py` tourne, n'importe quelle page du site peut appeler l'API normalement.

### Si une page ne s'affiche pas comme attendu

- **Une carte ou une section reste vide** : c'est normal si la fonction

Python ou JavaScript correspondante n'est pas encore codée. Les autres   sections de la page continuent de s'afficher normalement — seule la   section concernée reste vide en attendant votre code.

- **Un message d'erreur apparaît sur la page** : lisez-le, il indique

quelle fonction regarder. Le détail technique complet (traceback   Python) est toujours visible dans le terminal où tourne `python app.py`.

- **Rien ne s'affiche du tout** : vérifiez d'abord que le terminal de

l'API est bien ouvert et actif (pas d'erreur affichée dedans). Si vous   venez de modifier `main.js` ou `functions.js`, faites un rafraîchissement   forcé de la page (Ctrl+Maj+R ou Cmd+Maj+R) — le navigateur met parfois   en cache l'ancienne version du fichier.

## Qui fait quoi

| Parcours | Effectif | Vous complétez | Vous ne touchez PAS |
| --- | --- | --- | --- |
| **Data Science** | 1 à 3 personnes | `backend/logic.py` (17 fonctions) | `app.py`, `controllers.py` |
| **Full Stack** | 7 personnes | *voir répartition ci-dessous* | `main.js` |

**Le nommage des champs est déjà fixé dans le code** (docstrings de `logic.py`, structure de `data/trajets.json`, IDs des éléments HTML). Vous n'avez pas à deviner ces noms — regardez les docstrings et le jeu de données pour comprendre le contrat technique attendu.

## Répartition Full Stack

Chaque page est dans son propre sous-dossier avec son fichier CSS dédié. L'essentiel de votre note porte sur vos **pages HTML/CSS** (structure sémantique, box model, Flexbox/Grid, responsive mobile/tablette/desktop). Chacun complète aussi **2 fonctions JS** dans `frontend/functions.js`.

| Qui | Dossier & page | Fonctions JS |
| --- | --- | --- |
| Dev FS1 | `frontend/accueil/index.html` + `accueil.css` — page d'accueil, hero + indicateurs clés | `compterTrajetsAujourdhui`, `formaterQuartierPrincipal` |
| Dev FS2 | `frontend/recherche/recherche.html` + `recherche.css` — recherche et filtres | `filtrerParQuartierDepart`, `rechercherParMotCle` |
| Dev FS3 | `frontend/trajet/trajet.html` + `trajet.css` — détail d'un trajet + réservation | `formaterPrix`, `formaterHeure` |
| Dev FS4 | `frontend/proposer/proposer.html` + `proposer.css` — formulaire conducteur | `validerFormulaireProposer`, `formaterMessageConfirmation` |
| Dev FS5 | `frontend/mes-trajets/mes-trajets.html` + `mes-trajets.css` — historique passager | `filtrerReservationsParStatut`, `calculerTotalDepenseParPassager` |
| Dev FS6 | `frontend/dashboard/dashboard.html` + `dashboard.css` **ET** `frontend/confirmation/confirmation.html` + `confirmation.css` | `calculerPourcentageOccupation`, `getBadgeDisponibilite` |
| Dev FS7 | `frontend/inscription/inscription.html` + `inscription.css` **ET** `frontend/login/login.html` + `login.css` | `validerFormulaireInscription`, `validerFormulaireLogin` |

tin (7h-9h) et du soir (17h-19h).

Bonne construction.
