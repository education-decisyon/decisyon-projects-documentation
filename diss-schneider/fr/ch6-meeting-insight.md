---
icon: chart-line
---

# 6. Meeting Insight

### Overview

Meeting Insight est un agent IA qui travaille sur les réunions déjà capturées par MeetingSense. Tandis que MeetingSense se concentre sur un seul enregistrement, Meeting Insight analyse plusieurs transcriptions de réunions simultanément pour identifier les tendances, problèmes récurrents et actions agrégées dans l'ensemble des archives. Il transforme un flux de comptes-rendus SIM individuels en intelligence opérationnelle au niveau du site ou de la zone.

<figure><img src=".gitbook/assets/meeting-insight_action-items-list-aggregated-across-meetings.png" alt=""><figcaption></figcaption></figure>

## Quand l'utiliser

* Pour répondre à « Quels problèmes continuent de revenir ? » — Meeting Insight identifie les thèmes récurrents dans les réunions SIM sur une période choisie.
* Pour produire une liste consolidée d'actions issues de nombreuses réunions (ex. toutes les réunions SIM 1 du mois dernier) sans les ouvrir une par une.
* Pour extraire des tendances et des schémas sur différentes dates de production et zones de production, soutenant les revues de management et le pilotage de l'amélioration continue.
* Pour investiguer un sujet dans les archives de réunions en utilisant des questions en langage naturel dans n'importe quelle langue compatible.

## Prérequis

* Au moins une transcription de réunion produite par MeetingSense doit exister dans l'environnement DISS.
* L'utilisateur doit avoir accès aux archives Overview Meeting.
* L'utilisateur doit avoir accès en lecture aux réunions incluses dans l'analyse.

## Comment l'utiliser

{% stepper %}
{% step %}
### Naviguer vers les archives Overview Meeting

* Naviguer vers les archives **Overview Meeting** dans DISS.

<figure><img src=".gitbook/assets/meeting-insight_overview-meeting-archive-page.png" alt="Page des archives Overview Meeting"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Filtrer les archives de réunions

* Utiliser des filtres de date ou de niveau organisationnel pour isoler les réunions pertinentes pour le périmètre d'analyse.

<figure><img src=".gitbook/assets/meeting-insight_date-and-level-filters-on-the-archive.png" alt="Filtres de date et de niveau sur les archives"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Sélectionner les réunions à analyser

* Sélectionner plusieurs réunions en utilisant les cases à cocher à gauche de chaque ligne pour définir le jeu de données d'analyse.

<figure><img src=".gitbook/assets/meeting-insight_meetings-selected-via-checkboxes.png" alt="Réunions sélectionnées via les cases à cocher"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Lancer Meeting Insight

* Cliquer sur **Résumer les notes** pour lancer l'Agent Insight sur les réunions sélectionnées. L'agent ouvre une fenêtre de dialogue où il est possible d'interagir avec le jeu de données combiné de toutes les transcriptions sélectionnées.

<figure><img src=".gitbook/assets/meeting-insight_summarize-notes-button.png" alt="Bouton Résumer les notes"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Gérer la sélection active

* Utiliser le panneau latéral pour voir ou désélectionner des réunions spécifiques sans fermer le dialogue, en conservant le contrôle total sur le périmètre d'analyse.

<figure><img src=".gitbook/assets/meeting-insight_managing-the-active-selection-from-the-dialog.png" alt="Gestion de la sélection active depuis le dialogue"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Extraire la liste des actions

* Cliquer sur **Extraire la liste des actions** pour agréger toutes les actions des sessions sélectionnées en une seule liste.

<figure><img src=".gitbook/assets/meeting-insight_action-items-list-aggregated-across-meetings.png" alt="Liste des actions agrégée de plusieurs réunions"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Poser des questions en langage naturel

* Saisir des questions en langage naturel dans le champ de saisie pour localiser des détails opérationnels spécifiques — causes racines, obstacles récurrents, responsables — dans les transcriptions.

<figure><img src=".gitbook/assets/meeting-insight_natural-language-query-on-the-selected-meetings.png" alt="Requête en langage naturel sur les réunions sélectionnées"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Exporter et mettre en signet les résultats

* Mettre en signet les requêtes fréquemment utilisées pour une réutilisation plus rapide, et copier les résumés générés ou les listes d'actions dans des documents externes pour les rapports.

<figure><img src=".gitbook/assets/meeting-insight_bookmarking-a-query-and-exporting-the-results.png" alt="Mise en signet d'une requête et export des résultats"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lecture du résultat

| Résultat                        | Description                                                                                                                                                                          |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Liste des actions               | Une liste consolidée et dédupliquée de toutes les actions identifiées dans les sessions de réunion sélectionnées, avec description, responsable inféré et réunion source.             |
| Réponse en langage naturel      | Une réponse IA synthétisée basée sur le contenu transcrit complet des réunions sélectionnées, avec références à la réunion et session source.                                        |
| Requêtes mises en signet        | Requêtes fréquemment utilisées enregistrées et réutilisables depuis le panneau latéral, accélérant les analyses récurrentes comme les vérifications de tendances hebdomadaires.      |

{% hint style="info" %}
Les résultats sont indicatifs. Le chef de réunion reste responsable de transformer les tendances récurrentes en contre-mesures concrètes via la fonction Actions.
{% endhint %}

## Conseils et limites connues

{% hint style="info" %}
* La qualité des insights dépend de la qualité des comptes-rendus MeetingSense sous-jacents : encourager des enregistrements clairs et la mention explicite des responsables et des dates lors des réunions.
* Utiliser les filtres avant de lancer l'agent — analyser un jeu de données ciblé (ex. un niveau SIM et un mois) produit des insights plus précis qu'analyser l'ensemble des archives.
* La participation IA en temps réel pendant la réunion SIM elle-même ne fait pas partie de cette version : Meeting Insight opère aujourd'hui sur des comptes-rendus déjà enregistrés.
* Les insights sont indicatifs : le chef est responsable de traduire les tendances récurrentes en contre-mesures concrètes via des Actions ou des Katas.
{% endhint %}
