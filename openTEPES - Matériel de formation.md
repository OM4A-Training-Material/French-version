# ⚡ openTEPES

## 📚 Documentation et Matériel de Formation

Vous trouverez ici tout le nécessaire pour installer et exécuter **openTEPES** :

- 📖 [**Guide de l’utilisateur**](https://opentepes.readthedocs.io/en/latest/index.html) : Ce manuel en ligne comprend des sections détaillées sur :

  - Introduction
  - Données d’entrée pour les systèmes électriques, hydroélectriques, hydrogène et chaleur
  - Méthode d’intercouplage de marché basée sur les flux (Flow-Based Market Coupling)
  - Résultats de sortie
  - Formulation mathématique
  - Projets de recherche et publications
  - Téléchargement et installation
  - Questions & Réponses (Q&R)
  - Informations de contact

- 🛠️ [**Guide d’installation (PDF)**](openTEPES_InstallationGuide.pdf)

- 🧾 [**Présentation Résumée**](openTEPES_Summary.pdf)

- 🇫🇷 [**Résumé en français**](openTEPES_Resume.pdf)

- ❓ [**Résumé des Q&R**](openTEPES_QuestionsAndAnswers.pdf)

---

## 🧠 Aperçu du Modèle

Le modèle **openTEPES** est un système d’aide à la décision pour la **planification intégrée des ressources (IRP)**, combinant :

- Planification de l’expansion de la production (GEP)
- Planification de l’expansion du stockage (SEP)
- Planification de l’expansion du réseau de transport (TEP)

Il optimise les investissements dans la production, le stockage et la transmission sur des horizons temporels tactiques (10–20 ans), couvrant les réseaux d’électricité, d’hydrogène et de chaleur. Les utilisateurs définissent les projets candidats, et le modèle identifie les décisions d’investissement optimales.

---

## 🛠️ Installer openTEPES

Pour installer **openTEPES**, suivez ces étapes :

1. Installez [**Miniconda3**](https://docs.conda.io/en/latest/miniconda.html), qui inclut Python et d’autres packages essentiels.
2. Installez au moins un solveur compatible (par exemple : Gurobi, HiGHS).
3. Dans le terminal Anaconda, installez openTEPES avec la commande suivante :

```bash
pip install openTEPES
```

---

## 🚀 Exécuter openTEPES

1. Créez votre étude de cas personnalisée en adaptant l’un des exemples fournis (inclus dans le répertoire du modèle).
2. Ouvrez la console Anaconda et exécutez :

```bash
openTEPES_Main
```

3. Vous serez invité à :
   - Sélectionner le dossier contenant votre étude de cas
   - Nommer l’étude
   - Choisir le solveur
   - Définir les fichiers de sortie et de journalisation

---

## 🎥 Tutoriels Vidéo Pas-à-Pas

Vous pouvez trouver tous les tutoriels sur  
<a href="https://www.youtube.com/playlist?list=PLHN93NPePQ1KDpQpxvlpPTeDZPdePdHIL" target="_blank" style="text-decoration: none;">
  <img src="https://cdn.simpleicons.org/youtube/FF0000/16" alt="YouTube" height="16" style="vertical-align: text-bottom; margin-left: 4px;">
</a>

---

## ❓ Besoin d’aide ?

Consultez notre page [Questions & Réponses](docs/faq.md) pour les problèmes fréquents et les conseils pratiques.
