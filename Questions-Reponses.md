**Exercice 1 :**  
Quels sont les composants dont la perte entraîne une perte de données ?  
  
*..Répondez à cet exercice ici..*

**Exercice 2 :**  
Expliquez nous pourquoi nous n'avons pas perdu les données lors de la supression du PVC pra-data  
  
Alors techniquement on a perdu les données de la bdd de prod. Mais vus qu'il y a une backup représenté par le PVC pra-backup, les données peuvent être remise dans la bdd de base. La backup est mise à jour régulièrement via un cron et représente une copie de la bdd de prod. Et donc peut être poussé sur la bdd de prod quand un problème critique vient posé problème.

**Exercice 3 :**  
Quels sont les RTO et RPO de cette solution ?  
  
Environ de 1 à 3min pout le RTO et 2 jours pour le RPO

**Exercice 4 :**  
Pourquoi cette solution (cet atelier) ne peux pas être utilisé dans un vrai environnement de production ? Que manque-t-il ?   
  
*..Répondez à cet exercice ici..*
  
**Exercice 5 :**  
Proposez une archtecture plus robuste.   
  
*..Répondez à cet exercice ici..*