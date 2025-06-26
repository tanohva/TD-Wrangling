# TD-Wrangling
Voici le lien du dataset : https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

Etape 1 – Chargement & Nettoyage

1. Charger les fichiers suivants :
   
o olist_orders_dataset.csv

o olist_order_items_dataset.csv

o olist_order_reviews_dataset.csv

o olist_order_payments_dataset.csv

o olist_customers_dataset.csv

3. Vérifie s’il existe des doublons dans chaque fichier. Si oui, supprime-les.
   
5. Y a-t-il des valeurs manquantes dans les colonnes clés (dates, montants, identifiants) ? Traite-les de façon appropriée.
   
Etape 2 – Transformation des données

7. Calcule la durée de livraison pour chaque commande : order_delivered_customer_date - order_purchase_timestamp
   
9. Calcule l’écart entre la date estimée et la date réelle de livraison. Crée une variable binaire on_time_delivery qui vaut True si la commande a été livrée à temps ou en avance.
    
11. Calcule le montant total payé par commande (en fusionnant les paiements et les items).
    
13. Calcule le frais de port moyen par commande.
    
Etape 3 – Fusion et enrichissement

16. Crée une table finale contenant, pour chaque commande :
    
o ID client

o Date de commande

o Délai de livraison

o Estimation vs réel

o Score de satisfaction (review_score)

o Total payé

o Livraison à l’heure (oui/non)

17. Intègre les données clients pour ajouter le code postal à la table finale.
    
Etape 4 – Analyse exploratoire

19. Quelle est la répartition des scores de satisfaction (1 à 5) ?

20. Le délai de livraison a-t-il un impact sur la satisfaction ? Affiche la moyenne de review_score selon que la commande a été livrée à temps ou non.
    
22. Quel est le montant moyen des commandes selon le score de satisfaction ?
    
24. Quelles sont les 5 villes avec le plus de commandes livrées en retard ?
    
26. Quels sont les produits qui génèrent le plus de retards ?
    
28. Quel est le nombre moyen de jours de retard par catégorie de produit (product_category_name) ?
