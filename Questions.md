# Q1: Quels sont les arguments que vous pouvez utiliser pour convaincre votre Client de rendre son quizz accessible ? (Vous pouvez vous aider du cour)
Réponse:
Conformité légale : Respecter les normes d'accessibilité (RGAA, WCAG) pour éviter des sanctions.
Responsabilité sociale : Montrer un engagement envers l'inclusion et l'égalité des chances.
Augmentation de l’audience : Toucher une population plus large, y compris les personnes en situation de handicap.
Amélioration UX : Offrir une meilleure expérience utilisateur pour tous.
Meilleur référencement : Optimiser la visibilité grâce à un site bien structuré et accessible.
Fidélisation : Rendre le quiz utilisable par tous favorise la satisfaction et la fidélité des utilisateurs.
# Q2: Ajouter le screen de votre score :
Screen:![alt text](image.png)
Le score obtenu pour l'accessibilité avec Lighthouse est de 67/100
# Q3: Est-ce que l'analyse de Lighthouse est suffisante pour évaluer l'Accessibilité de votre Application ?
Réponse:
L'analyse de Lighthouse n'est pas suffisante pour évaluer complètement l'accessibilité de l'application. Voici pourquoi :

Limites de Lighthouse :

Lighthouse se base sur des tests automatisés qui détectent des problèmes évidents, mais il ne peut pas identifier tous les problèmes d'accessibilité, en particulier ceux qui nécessitent une analyse manuelle (exemple : pertinence des descriptions ou de l'ordre de navigation).
Importance des tests manuels :

Certains aspects comme l’expérience utilisateur avec un lecteur d’écran, la clarté des contenus ou les interactions clavier nécessitent des tests humains.
Recommandation complémentaire :

Pour une évaluation complète, il est essentiel de combiner Lighthouse avec :
Des outils comme Axe ou Wave pour des tests approfondis.
Des tests manuels avec des utilisateurs en situation de handicap.
Une revue des standards WCAG (Web Content Accessibility Guidelines).
En conclusion, Lighthouse est un bon point de départ, mais une évaluation approfondie nécessite d’autres outils et des tests humains.

# Q4: Combien de fois vous devez utiliser une touche du clavier pour passer le quizz ?
Réponse:
Environ 20 TAB pour les icônes des réseaux sociaux.
Ensuite, pour chaque question :
1 TAB par bouton de réponse (ex. Brésil, Colombie, Finlande).
Si vous avez 3 questions avec 4 réponses par question, cela fait :
20 + (3×4) = 32 tab


20+(3×4)=32TAB.
Conclusion : Il faut environ 32 TAB pour parcourir ce quiz de 3 questions, en tenant compte des réseaux sociaux et des options de réponse.
# Q5: Donner 3 roles ARIA et 3 propriété ARIA
Réponse:
3 rôles ARIA :

role="button" : Définit un élément interactif comme un bouton.
role="alert" : Utilisé pour afficher un message d'alerte qui est immédiatement annoncé par les lecteurs d’écran.
role="navigation" : Indique une section de la page contenant des liens de navigation.
# Q6: Ajouter le screen de votre score Lighthouse
Screen:
![alt text](image-1.png)
Le score d'accessibilité est passé de 67 à 71, ce qui représente une légère amélioration. Cependant, des problèmes persistent, notamment :

Absence d'attribut alt pour les images, ce qui empêche les lecteurs d'écran de décrire les images.
Les liens n'ont pas de noms visibles, rendant la navigation difficile sans souris, surtout avec l'utilisation de la touche TAB pour passer d'un élément à un autre.
Ces erreurs affectent l'expérience utilisateur, particulièrement pour ceux qui naviguent uniquement au clavier.
# Q7: L'une des best practice de l'ARIA est "ne pas utiliser l'ARIA" pouvez nous expliquer pourquoi d'après vous ?
Réponse:
L'une des meilleures pratiques de l'ARIA est "ne pas utiliser l'ARIA" car les éléments HTML sémantiques natifs sont déjà optimisés pour l'accessibilité et intégrés aux navigateurs. Voici pourquoi :

HTML sémantique est suffisant :

Les balises comme <button>, <nav>, <header> ou <footer> possèdent déjà des rôles ARIA par défaut.
Par exemple, <button> a automatiquement le rôle role="button" sans nécessiter d'attribut ARIA supplémentaire.
Éviter les conflits :

Ajouter des rôles ARIA redondants sur des éléments HTML natifs peut entraîner des conflits avec les lecteurs d'écran.
Exemple : <button role="button"> est inutile et peut causer des problèmes d'interprétation.
Performance et maintenance :

Utiliser des balises HTML sémantiques simplifie le code et améliore la maintenance. Ajouter inutilement ARIA complexifie le code sans gain réel.
Priorité aux standards :

ARIA doit être utilisé uniquement lorsque les éléments HTML natifs ne suffisent pas, comme pour des composants complexes créés avec JavaScript.
# Q8: Ajouter le screen de votre score Lighthouse
Screen:
![alt text](image-2.png)
Le score d’accessibilité est maintenant de 95, ce qui représente une nette amélioration par rapport au score initial de 67 et 71.

Explication :
Utilisation des balises HTML sémantiques :

Les balises <header>, <main>, <section>, <nav> et <footer> permettent une meilleure structure logique de la page.
Elles intègrent des rôles ARIA par défaut, améliorant la compréhension pour les lecteurs d’écran.
# Q9: Pourquoi le score de lighthouse n'a pas augmenté d'après vous ?
Réponse:

# Q10: Quel est la valeur du rapport de contraste actuel :
Réponse:
La valeur actuelle du rapport de contraste est de 2,38, ce qui est insuffisant par rapport aux normes d'accessibilité (minimum 4,5:1 pour AA).
# Q11: Quel est la valeur du score AA :
Réponse:
La valeur du score AA correspond à un rapport de contraste de 4.5:1 pour le texte normal et 3:1 pour le texte large.
# Q12: Quel est la valeur du score AAA :
Réponse:
La valeur du score AAA correspond à un rapport de contraste de 7:1 pour le texte normal et 4.5:1 pour le texte large.
# Q13: Comment pouvez vous changer la valeur du contraste de votre texte ?
Réponse:
Modifier la couleur du texte et de l’arrière-plan dans le fichier CSS afin d'augmenter la différence entre les deux :

# Q14: Ajouter le screen de votre score Lighthouse
Screen:
![alt text](image-3.png)
Par exemple, au lieu d'utiliser la couleur gray, j'ai utilisé le code couleur #b5b5b5 pour obtenir un meilleur contraste.
# Q15: Êtes vous capable de déterminer visuellement ce qui est un lien ou pas en appliquant chaque altérations ?
![alt text](image-4.png)
Non, il est difficile de déterminer visuellement ce qui est un lien ou non après avoir appliqué chaque altération. Voici les observations pour chaque cas :

Vision floue : Les liens deviennent indistincts et se confondent avec le texte ordinaire.
Achromatopsie : Les couleurs ne sont plus visibles, donc les liens ne se démarquent pas s'ils ne sont pas soulignés.
Daltonisme : Les différences de couleur entre les liens et le texte sont souvent perdues, rendant leur identification compliquée.
# Q16: Ajouter le screen de votre score Lighthouse
Screen:
![alt text](image-5.png)
Le score de 100.
# Q17:  Proposition 1
Ajout de l'attribut aria-live="polite" à l'élément contenant les questions, ce qui permet aux lecteurs d'écran d'annoncer automatiquement les nouvelles questions lorsqu'elles apparaissent. Cette amélioration facilite l'interaction des utilisateurs de technologies d’assistance en réduisant le nombre d'actions nécessaires, car :

Les utilisateurs n'ont plus à naviguer jusqu'à l'élément pour entendre la question.
Les mises à jour de la question sont détectées et lues de manière automatique.
Nombre d'actions supprimées :
1 à 2 actions par question, soit une réduction totale de 10 à 20 actions sur un quiz de 10 questions.
# Q18:  Proposition 2
Description :
Ajout d'une fonctionnalité permettant aux lecteurs d'écran (comme le Narrateur de Windows) de lire automatiquement les questions. Cette amélioration, qui n'était pas présente auparavant, a été mise en place grâce à :

L'intégration de aria-live="polite" sur l'élément contenant les questions, afin de notifier les lecteurs d'écran des mises à jour.
Une réinitialisation et une réinsertion du texte des questions via innerText avec un léger délai, permettant de forcer la détection du changement.
La temporisation de l'affichage des réponses à l'aide de aria-hidden="true", garantissant que les questions sont lues avant les réponses.
Nombre d'actions gagnées :
1 action par question, soit une économie totale de 10 actions pour un quiz de 10 questions.

# Q19:  Proposition 3
Description:
Description: Mettre les liens en fin de page, et peut etre meme ignorer les question pour le narrateur
Nb d'actions gagnée : 
