# InfraFair
*"Équité dans la répartition des coûts d'infrastructure"*   

**InfraFair** a été développé à l’[Instituto de Investigación Tecnológica (IIT)](https://www.iit.comillas.edu/index.php.en) 
de l’[Universidad Pontificia Comillas](https://www.comillas.edu/en/).

- 📖 [**Documentation Complète**](https://infrafair.readthedocs.io/en/latest/index.html)
- 💻 [**Projet GitHub**](https://github.com/IIT-EnergySystemModels/InfraFair/tree/main)
- 🐍 Langage : Python 3

---

## 🧠 Aperçu du Modèle

InfraFair est un outil de modélisation conçu pour calculer la répartition des coûts des infrastructures énergétiques 
selon l'utilisation économique anticipée par les agents, afin d’orienter efficacement les décisions d’investissement.  
InfraFair détermine l'utilisation du réseau par les agents, les opérateurs de système et les pays.  
Sur cette base, et en supposant que l’utilisation reflète les bénéfices économiques reçus, 
il attribue la responsabilité de chaque élément du réseau à chaque agent.  
Il peut également attribuer les pertes aux agents responsables.

---

## 📚 Matériel de Formation

- 🛠️ [**Guide d'Installation (PDF)**](Guide_for_installing_Python_and_InfraFair.pdf)

- 🧾 [**Présentation Résumée**](InfraFair_Introduction.pdf)

- ❓ [**FAQ Résumée**](InfraFair_Q&A.pdf)

---

## ⚙️ Installation

InfraFair peut être facilement installé avec pip :

      > pip install InfraFair 

Alternativement, suivez ces quatre étapes via GitHub :

1. Clonez le dépôt InfraFair contenant la structure et les fonctions nécessaires.
2. Lancez l’invite de commande (Windows : Win+R, tapez "cmd") ou le terminal Anaconda.
3. Placez-vous dans le répertoire du dépôt :

         > cd "C:\\Users\\<nom_utilisateur>\\...\\InfraFair"
4. Installez InfraFair via pip :

         > pip install . 

Pour mettre à jour une version existante :

      > pip install --upgrade InfraFair 

---

## 🚀 Exécuter InfraFair

Une fois installé, InfraFair peut être lancé via une invite de commande. 
Dans le répertoire de votre choix, ouvrez et exécutez le script InfraFair.py :

    > python InfraFair.py

Trois paramètres vous seront demandés (répertoire, nom de cas, fichier de configuration).

**Remarque** : Appuyez simplement sur Entrée à chaque question pour utiliser les valeurs par défaut.

Ensuite, copiez le [simple exemple](<https://github.com/IIT-EnergySystemModels/InfraFair/tree/main/Examples/Simple_ex>) ou 
[l’exemple UE](<https://github.com/IIT-EnergySystemModels/InfraFair/tree/main/Examples/EU_ex>) dans un nouveau dossier, et utilisez-le comme base.

Les résultats seront enregistrés dans le même dossier que les fichiers d’entrée.

**Note** : Vous pouvez aussi créer un nouveau script **script.py** avec le contenu suivant :
        
```python
from InfraFair import InfraFair_run
        
InfraFair_run(<dir>, <cas>, <fichier_config>)
