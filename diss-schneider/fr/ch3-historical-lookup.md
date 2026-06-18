---
icon: clock-rotate-left
---

# 3. Recherche Historique

### Aperçu général

**Recherche Historique** est une fonctionnalité IA qui, à partir du Kata QRCI en cours de traitement, recherche les Katas clôturés du même site et renvoie les plus similaires. Pour chaque Kata historique, l'utilisateur peut consulter l'explication IA sur la correspondance et importer — sélectivement — les actions qui ont été utilisées pour résoudre le problème passé, accélérant la réponse face aux problèmes récurrents.

<figure><img src=".gitbook/assets/historical-lookup_ai-analysis-accordion-expanded.png" alt=""><figcaption></figcaption></figure>

## Quand l'utiliser

* Quand un problème en usine semble familier mais que l'équipe ne se souvient plus quand, où et comment il a été résolu.
* Avant d'enregistrer un nouveau Kata, pour vérifier si le même problème a déjà été traité et éviter de dupliquer les efforts.
* Lors de l'analyse des causes racines, pour lire comment les collègues ont formulé l'État Actuel et l'État Cible dans un cas comparable.

## Prérequis

* Le Kata actuel doit avoir un Site défini : Recherche Historique ne s'active que lorsque le Site est configuré.
* Il doit exister au moins un Kata avec le statut **Clôturé** dans le périmètre de recherche pour que l'IA trouve des correspondances.
* L'utilisateur doit avoir accès en lecture aux Katas historiques dans le périmètre de recherche.

## Comment l'utiliser

{% stepper %}
{% step %}
### Ouvrir le tableau de bord Kata

* Ouvrir le **tableau de bord Kata** dans DISS.

<figure><img src=".gitbook/assets/historical-lookup_kata-dashboard-with-the-ai-tools-column-visible.png" alt="Tableau de bord Kata avec la colonne des outils IA visible"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Lancer Recherche Historique

* Dans la colonne **Kata**, cliquer sur l'**icône de similarité Kata** à côté du Kata Ouvert en cours de traitement.

<figure><img src=".gitbook/assets/historical-lookup_icon-highlighted-on-a-kata-row.png" alt="Icône de similarité Kata mise en évidence sur une ligne Kata"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Attendre la fin de la recherche IA

* La modale **AI Recherche Historique** s'ouvre et la recherche démarre automatiquement — aucune saisie supplémentaire n'est requise. Attendre la fin du message de chargement (« Chargement des Katas similaires… »).

<figure><img src=".gitbook/assets/historical-lookup_modal-in-loading-state.png" alt="Modale Recherche Historique en état de chargement"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Consulter les Katas similaires

* Consulter les jusqu'à 5 Katas clôturés renvoyés, triés par score de similarité décroissant.

<figure><img src=".gitbook/assets/historical-lookup_list-of-matches-with-similarity-scores.png" alt="Liste des correspondances avec scores de similarité"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Analyser chaque correspondance en détail

* Pour chaque correspondance, développer l'accordéon **Analyse IA** pour lire « **Pourquoi ça correspond** » et « **Différences à considérer** ».

<figure><img src=".gitbook/assets/historical-lookup_ai-analysis-accordion-expanded.png" alt="Accordéon Analyse IA développé"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Copie sélective des actions

Chaque correspondance historique dispose d'un sélecteur **Actions réutilisables**. Lorsqu'il est développé, les actions de ce Kata se chargent et une case à cocher apparaît à côté de chaque action. Il est possible de :

* Sélectionner des actions individuelles une par une ;
* Utiliser **Tout sélectionner / Tout désélectionner** au sein d'un Kata historique ;
* Combiner des sélections provenant de plusieurs Katas dans la même session — le compteur total est toujours visible.

Lorsqu'au moins une action est sélectionnée, le bouton **Importer N actions** apparaît en bas. Cliquer dessus pour copier les actions sélectionnées dans le Kata actuel. Pour chaque action importée :

* Le **Titre** et la **description** sont copiés depuis la source ;
* Le statut est réinitialisé à Ouvert ;
* La date limite par défaut est aujourd'hui + 7 jours ; le nouveau responsable définit une nouvelle date.

À la fin, la modale se ferme automatiquement, un message de confirmation apparaît et le tableau des Actions du Kata actuel est mis à jour pour afficher les nouveaux enregistrements.

{% stepper %}
{% step %}
### Charger les actions historiques

* Dans l'une des correspondances, cliquer sur **Actions réutilisables** pour charger les actions historiques de ce Kata.

<figure><img src=".gitbook/assets/selective-action-copy_view-actions-toggle-expanded-for-a-match.png" alt="Sélecteur Actions réutilisables développé pour une correspondance"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Sélectionner les actions à importer

* Utiliser les cases à cocher pour sélectionner des actions individuelles, ou utiliser **Tout sélectionner / Tout désélectionner** pour agir sur l'ensemble du Kata.

<figure><img src=".gitbook/assets/Selective Action Copy — checkboxes and Select All - Deselect All controls.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Combiner des sélections de plusieurs Katas

* Répéter optionnellement pour d'autres correspondances : la sélection persiste entre plusieurs Katas dans la même session.

<figure><img src=".gitbook/assets/selective-action-copy_multi-kata-selection-with-total-counter-visible.png" alt="Sélection multi-Katas avec compteur total visible"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Importer les actions sélectionnées

* Cliquer sur **Importer N actions** en bas de la modale.

<figure><img src=".gitbook/assets/Selective Action Copy — Import N Actions button.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirmer et vérifier les actions importées

* La modale se ferme, une confirmation apparaît et le tableau des Actions du Kata actuel est mis à jour avec les nouveaux enregistrements (Statut = Ouvert, Date limite = Date du jour).

<figure><img src=".gitbook/assets/selective-action-copy_current-kata-actions-table-refreshed-with-imported-records.png" alt="Tableau des Actions du Kata actuel mis à jour avec les enregistrements importés"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lecture du résultat

| Champ                    | Description                                                                                                                                                                                   |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Score de similarité      | Un pourcentage (0–100) indiquant dans quelle mesure le Kata clôturé correspond au Kata ouvert. Des scores supérieurs à 70 indiquent un fort chevauchement thématique ; inférieurs à 40 sont des correspondances faibles affichées pour être complet. |
| Pourquoi ça correspond   | Une explication concise générée par l'IA des éléments partagés entre les deux Katas.                                                                                                         |
| Différences à considérer | Un bref résumé de ce qui distingue le cas historique du cas actuel.                                                                                                                           |
| Actions réutilisables    | La liste complète des actions du Kata historique, prêtes pour une importation sélective.                                                                                                      |

## Conseils et limites connues

{% hint style="info" %}
* Par défaut, Recherche Historique recherche uniquement dans le site actuel. Lorsque le périmètre multi-site est activé, le site d'origine est clairement indiqué sur chaque résultat.
* Seuls les Katas **Clôturés** sont pris en compte ; les Katas en cours sont exclus.
* Les Katas identiques ou quasi identiques ne sont pas masqués — ils apparaissent avec une similarité très élevée pour que vous puissiez décider d'importer leurs actions.
* Les actions importées repartent toujours de zéro (Statut = Ouvert, Date limite = par défaut aujourd'hui + 7 jours) : le nouveau responsable prend en charge le délai.
* Les filtres Zone, Ligne, Origine et KPI ne sont PAS des filtres stricts — l'IA les utilise comme contexte sémantique, ce qui signifie qu'une correspondance pertinente d'une Ligne différente peut toujours être proposée.
{% endhint %}
