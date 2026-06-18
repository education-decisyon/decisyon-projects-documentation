---
icon: microphone
---

# 5. Meeting Sense

### Aperçu général

**Meeting Sense** est la capacité d'enregistrement et de transcription de réunions intégrée dans DISS. Elle transforme le dialogue oral d'une réunion SIM en données numériques structurées : une transcription textuelle, un résumé exécutif, les problèmes soulevés et une liste d'actions proposées prêtes à être ajoutées au plan d'action SIM. La session est automatiquement contextualisée avec les métadonnées du SIM Board depuis lequel elle a été lancée (Site, niveau SIM, Zone de production) pour que chaque résultat soit déjà lié au bon périmètre opérationnel.

<figure><img src=".gitbook/assets/recording-widget-in-active-state-during-the-meeting-with-session-duration-and-audio-status-indicator.png" alt=""><figcaption></figcaption></figure>

## Quand l'utiliser

* Lors d'une réunion quotidienne SIM 2 où l'équipe discute de problèmes, causes racines et actions correctives et souhaite que chaque résultat soit traçable dans DISS sans prise de notes manuelle.
* Quand le Chef SIM veut que la conversation soit intégralement enregistrée pour que rien ne soit perdu entre la discussion et le plan d'action.
* Quand l'équipe a besoin à la fois d'un registre de présence et d'un ensemble structuré d'actions prêtes à assigner en une fois en fin de réunion.

## Prérequis

* Le SIM Board dans lequel la réunion est ouverte doit être un **SIM 2** Board (Meeting Sense est activé à ce niveau SIM).
* Un microphone fonctionnel doit être disponible sur l'appareil utilisé pour démarrer la réunion.
* Les rôles de présence doivent être configurés pour le SIM 2 Board — accessible dans **Configuration du site → Présence → Configuration de la présence SIM 2.**
* L'utilisateur doit avoir la permission de démarrer une réunion sur le SIM Board concerné.

## Comment l'utiliser

{% stepper %}
{% step %}
### Ouvrir le SIM Board et démarrer la réunion

* Naviguer vers le SIM Board où se tient la réunion (**Digitized Idea & SIM System → SIM Boards → SIM 2**). Le Site, la Zone de production et la Date sont renseignés automatiquement.
* Cliquer sur **Démarrer la réunion** en haut à droite pour ouvrir le dialogue d'initialisation.

<figure><img src=".gitbook/assets/sim-board-with-start-meeting-button-highlighted-in-the-top-right-corner.png" alt="SIM Board avec le bouton Démarrer la réunion mis en évidence"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Initialiser la présence et le Chef SIM

Dans le dialogue d'initialisation :

* Définir le statut de chaque participant (**À l'heure, En retard, Absent** ou **Non requis**) ;
* Assigner le **Chef SIM** (par défaut l'utilisateur actuel, modifiable via liste déroulante) ;
* Cliquer sur **Démarrer la réunion** pour continuer.

<figure><img src=".gitbook/assets/meeting-initialisation-dialog-attendance-statuses-and-sim-leader-selector.png" alt="Dialogue d'initialisation avec statuts de présence et sélecteur Chef SIM"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Sélectionner l'entrée audio et démarrer l'enregistrement

* Choisir le microphone souhaité dans la liste des entrées audio disponibles et confirmer. Si aucun microphone n'est détecté, un message d'erreur s'affiche et l'enregistrement ne peut pas démarrer.

<figure><img src=".gitbook/assets/audio-input-device-selection-popup-with-a-microphone-confirmed.png" alt="Popup de sélection du périphérique audio avec microphone confirmé"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Tenir la réunion

Parler clairement tout au long de la réunion et articuler les éléments nécessaires à la création d'actions :

* Une **brève description** du problème ;
* La **Catégorie** concernée (Sécurité, Qualité, Livraison, Maintenance, Production, Ingénierie) ;
* Le **nom de la personne assignée** ;
* La date **cible** de clôture.

<figure><img src=".gitbook/assets/recording-widget-in-active-state-during-the-meeting-with-session-duration-and-audio-status-indicator.png" alt="Widget d'enregistrement en état actif, avec durée de session et indicateur d'état audio"><figcaption></figcaption></figure>

{% hint style="info" %}
Un délai d'expiration prédéfini protège contre les réunions laissées ouvertes par erreur : un dialogue de notification apparaît deux minutes avant l'expiration pour permettre de prolonger ou d'arrêter manuellement la session.
{% endhint %}
{% endstep %}

{% step %}
### Arrêter l'enregistrement

* Cliquer sur le contrôle **Arrêter** lorsque la réunion est terminée. Le système commence à traiter l'audio en arrière-plan. Pendant la génération de la transcription, il est possible de passer à d'autres activités — l'équipe n'a pas besoin d'attendre sur la page de réunion.
* Une notification confirme quand la transcription et l'analyse IA sont prêtes.

<figure><img src=".gitbook/assets/recording-stopped-processing-indicator-and-confirmation-that-transcription-is-queued.png" alt="Enregistrement arrêté, indicateur de traitement et confirmation que la transcription est en file d'attente"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Ouvrir la réunion depuis les archives

* Naviguer vers **Réunion → Overview Meeting**.
* La page Overview Meeting liste chaque session enregistrée par ordre chronologique, affichant le titre, le niveau SIM, la date et le Chef SIM.

<figure><img src=".gitbook/assets/overview-meeting-archive-with-the-list-of-recorded-sessions.png" alt="Archives Overview Meeting avec la liste des sessions enregistrées"><figcaption></figcaption></figure>

* Cliquer sur une réunion pour ouvrir sa vue détaillée.

<figure><img src=".gitbook/assets/meeting-detail-view_summary-identified-issues-ai-suggested-actions.png" alt="Vue détaillée de la réunion : Résumé, Problèmes identifiés, Actions suggérées par l'IA, durée, registre de présence"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Consulter et modifier la transcription

* Cliquer sur **Afficher la transcription** pour afficher le texte littéral, qui reste entièrement modifiable.
* Corriger toute interprétation erronée du moteur de reconnaissance vocale ou ajouter des détails non capturés.
* Lorsque la transcription est mise à jour, cliquer sur **Générer les notes de réunion** pour actualiser le résumé IA.

<figure><img src=".gitbook/assets/transcript-pane-with-show-transcription-opened-and-generate-meeting-notes-button.png" alt="Panneau de transcription avec Afficher la transcription ouvert et le bouton Générer les notes de réunion"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lecture du résultat

| Bloc                          | Description                                                                                                                                           |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| Résumé                        | Une vue d'ensemble narrative de la discussion de réunion générée par l'IA, couvrant les principaux sujets abordés.                                   |
| Problèmes identifiés          | Une liste structurée de problèmes et anomalies identifiés lors de la réunion, extraits par l'IA de la conversation enregistrée.                       |
| Actions suggérées par l'IA   | Propositions d'actions générées automatiquement à partir du dialogue, chacune avec une description inférée, une catégorie, un responsable et une date limite. |
| Registre de présence          | La liste de présence compilée au début de la réunion, avec le statut défini pour chaque participant.                                                   |
| Durée                         | La durée totale de la session de réunion enregistrée.                                                                                                 |

## Conseils et limites connues

{% hint style="info" %}
* Parler clairement et éviter les voix qui se chevauchent : la qualité de l'extraction IA augmente avec la clarté de l'audio.
* Mentionner les noms et les dates avec précision — « Jean, pour vendredi » produit une suggestion IA plus solide que des références implicites comme « lui, pour ce week-end ».
* La Catégorie et le Responsable sont obligatoires pour la création d'actions : une action proposée sans ces valeurs doit être complétée dans le tableau de validation avant de pouvoir être enregistrée.
* Meeting Sense est un assistant d'enregistrement : le Chef SIM garde toujours le contrôle — les actions font partie du plan SIM uniquement après validation explicite, et la transcription peut être modifiée et résumée à nouveau avant de créer des actions.
{% endhint %}
