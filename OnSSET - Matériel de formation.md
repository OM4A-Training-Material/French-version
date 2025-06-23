# 🛠️ OnSSET

OnSSET est un outil de planification de l'électrification basé sur les Systèmes d’Information Géographique (SIG), conçu pour évaluer les trajectoires les moins coûteuses vers un accès universel à l’électricité. Il modélise des scénarios spatiaux explicites qui combinent la distribution de la population, les infrastructures et les données sur les énergies renouvelables afin de proposer les options d’électrification les plus économiques pour chaque localité. L’outil prend en charge à la fois l’extension du réseau centralisé et les solutions décentralisées hors réseau, à moyen et long terme.

OnSSET est composé de :

- Un noyau de modélisation basé sur Python qui exécute les simulations de scénarios et l’optimisation  
- Une suite de plugins QGIS pour prétraiter les données spatiales et générer les entrées du modèle  
- Des fichiers CSV de sortie décrivant les stratégies d’électrification et les métriques de coûts au niveau des localités  
- Des outils de visualisation pour explorer, cartographier et comparer les résultats entre scénarios

## 📄 Documentation

Voici tout ce qu’il vous faut pour installer et utiliser OnSSET :

[Guide d’installation d’OnSSET](./Installation%20Guide%20for%20OnSSET.pdf)  
Ce document PDF comprend :
- Un guide d’installation pour Windows, Linux et macOS
- Comment créer un environnement virtuel Python et installer les bibliothèques nécessaires
- Instructions pour installer QGIS et les plugins OnSSET
- Liens vers le dépôt GitHub officiel et la documentation d’OnSSET

[Guide de configuration des données pour OnSSET](./Data%20configuration%20Guide%20for%20OnSSET.pdf)  
Ce PDF explique :
- Comment préparer les clusters de population et les couches spatiales (ex. routes, réseaux, solaire, éolien, éclairage nocturne)
- Sources de données recommandées pour les couches SIG
- Guide étape par étape pour configurer le fichier `CountrySpecs.xlsx`
- Comment définir les paramètres de scénario dans les scripts Python

[Fichiers de sortie dans OnSSET](./Output%20files%20in%20OnSSET.pdf)  
Ce PDF contient :
- Explication des différents types de fichiers générés par OnSSET
- Conventions de nommage des scénarios et structures des fichiers
- Comment interpréter les résultats d’électrification et les métriques de coûts
- Liens avec les conventions de nommage des scénarios OpenModAfrica

[Description des colonnes de sortie](./Description-of-output-columns_OnSSET.pdf)  
Ce PDF fournit :
- Une liste détaillée de toutes les colonnes des fichiers CSV de résultats
- Unités et définitions de chaque variable (ex. population, demande, LCOE, investissement, distance au réseau)
- Conseils pour interpréter les valeurs liées aux niveaux de demande, au statut du réseau et aux choix technologiques

[Guide des cartes de sortie](./Maps%20output.pdf)  
Ce PDF montre :
- Comment charger et visualiser les résultats OnSSET dans QGIS ou ArcGIS
- Étapes pour créer des cartes ponctuelles à partir des fichiers CSV
- Comment classer, symboliser et exporter les cartes pour les rapports et présentations

## 🎥 Tutoriels Vidéo Pas-à-Pas

Vous pouvez retrouver tous les tutoriels sur  
<a href="https://www.youtube.com/playlist?list=PLHN93NPePQ1JNz3JROb_sVbF5pjOG-EDx" target="_blank" style="text-decoration: none;">
  <img src="https://cdn.simpleicons.org/youtube/FF0000/16" alt="YouTube" height="16" style="vertical-align: text-bottom; margin-left: 4px;">
</a>

## 💡 Support supplémentaire
### Installer OnSSET

Pour installer OnSSET :
- Suivez le [Guide d’installation](./Installation%20Guide%20for%20OnSSET.pdf)  
- Clonez le dépôt : [https://github.com/OnSSET/onsset](https://github.com/OnSSET/onsset)  
- Installez les dépendances :
  - pip install -e .
  - pip install numpy pandas geopandas matplotlib scikit-learn
- Installez QGIS et les plugins OnSSET :
  - [Plugin Population Clustering](https://github.com/OnSSET/PopCluster)
  - [Plugin GEP](https://github.com/OnSSET/ClusterbasedExtraction)

### Exécuter OnSSET

1. Préparez les couches d’entrée et le fichier `CountrySpecs.xlsx`
2. Définissez les paramètres dans `runner.py`
3. Lancez le modèle :
```bash
python runner.py
```

### ❓ Besoin d’aide ?

Consultez notre page [Questions & Réponses](docs/faq.md) pour les problèmes fréquents et les conseils utiles.

---

Références :  
Dépôt officiel : [https://github.com/OnSSET/onsset](https://github.com/OnSSET/onsset)  
Documentation : [https://onsset.readthedocs.io/](https://onsset.readthedocs.io/)
