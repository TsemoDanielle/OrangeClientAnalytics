# OrangeClientAnalytics - Summer Challenge 2025

##  Nom / Prénom
Nguemthueng Tsemo Bibiane Danielle
##  Structure du dépôt

```
    dataset_clients_orange.csv            jeu de données
    OrangeClientAnalytics.ipynb           notebook complet (exécutable sur Colab )
rapport_OrangeClientAnalytics.pdf  rapport synthétique
README.md
```

##  Instructions pour la préparation des données et l’exécution

###  Option 1 : Depuis **Google Colab** 

1. Aller sur : https://colab.research.google.com/
2. Cliquez sur "GitHub" et cherchez ce dépôt : `TsemoDanielle/OrangeClientAnalytics`
3. Ouvrez le fichier : `OrangeClientAnalytics.ipynb`
4. Connectez votre Google Drive pour accéder aux données :
```python
from google.colab import drive
drive.mount('/content/drive')
```
5. Modifiez le chemin du fichier CSV  :
```python
file_path = "/content/drive/MyDrive/dataset_clients_orange.csv"
```
6. Exécutez les cellules **dans l’ordre**

---

###  Option 2 : Depuis votre PC avec **Jupyter Notebook**

1. Cloner le dépôt :
```bash
git clone https://github.com/TsemoDanielle/OrangeClientAnalytics.git
```
2. Ouvrir le terminal ou Anaconda et lancer :
```bash
jupyter notebook
```
3. Ouvrir `OrangeClientAnalytics.ipynb`
4. Exécutez les cellules dans l’ordre
## Librairies utilisées
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Résumé des observations
- Les clients sont répartis dans 5 régions, avec une concentration dans l’Adamaoua et le Centre.
- Deux types de forfaits sont présents : prépayé (70%) et postpayé (30%).
- La majorité des clients consomment entre 1000 et 2000 Mo de data.
- Les clients postpayés ont en moyenne des factures plus élevées.
- Trois segments de clients ont été identifiés via KMeans :
  - Cluster 0 : utilisateurs modérés, forte utilisation des SMS
  - Cluster 1 : profils mixtes, usage équilibré
  - Cluster 2 : gros consommateurs de data avec facture modérée

##  Recommandations business
- **Identifier les clients à forte consommation data mais petite facture** pour proposer des migrations vers des forfaits plus adaptés.
- **Proposer des migrations de prépayé vers postpayé** pour les clients du cluster 1 (profils mixtes).
- **Créer des offres SMS personnalisées** pour les clients du cluster 0 (forts utilisateurs de messages).
- **Cibler géographiquement** les offres marketing dans les régions les plus représentées.

##  Ce qui aurait pu être ajouté avec plus de temps
- Analyse temporelle de la consommation (sur plusieurs mois)
- Segmentation plus fine avec DBSCAN ou t-SNE
- Enrichissement des données avec des informations sur les modèles de téléphone, ou la profession du client
