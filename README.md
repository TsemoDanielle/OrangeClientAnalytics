# OrangeClientAnalytics - Summer Challenge 2025

##  Nom / Prénom
Nguemthueng Tsemo Bibiane Danielle

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
