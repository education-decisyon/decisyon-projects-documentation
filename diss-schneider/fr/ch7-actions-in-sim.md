---
icon: list-check
---

# 7. Actions in SIM

### Aperçu général

La fonctionnalité **Actions** dans DISS est la manière structurée d'enregistrer, d'assigner et de suivre les activités correctives et d'amélioration directement depuis les SIM Boards. Deux cas d'usage complémentaires sont documentés ici : **Créer une action** — pour enregistrer une nouvelle action avec tout le contexte SIM — et **Modifier une action** — pour maintenir une action existante à jour pendant que l'équipe la résout dans la routine quotidienne SIM.

<figure><img src=".gitbook/assets/Action - Overview (1).png" alt=""><figcaption></figcaption></figure>

## Quand l'utiliser

* Ouvrir une **Créer une action** lors d'une réunion SIM quand un problème ou une opportunité est identifié sur la ligne : un problème Sécurité / Qualité / Livraison / Maintenance / Production / Ingénierie avec un responsable clair et une date limite.
* Ouvrir une **Modifier une action** entre les réunions SIM pour maintenir une action à jour : progression du statut, description affinée, nouvelles pièces jointes, solutions capturées ou notes ajoutées au Journal d'activité.
* Utiliser Actions in SIM pour s'assurer que chaque problème identifié sur un SIM Board devient une activité traçable et assignable, plutôt qu'un engagement verbal.

## Prérequis

* L'utilisateur doit avoir accès aux SIM Boards sur lesquels les Actions sont activées.
* Les catégories d'action, zones de production et lignes doivent être configurées dans **Configuration du site** — elles alimentent les champs Catégorie, Module et Ligne dans le formulaire Créer une action.
* Le Responsable ou l'Équipe doit exister dans DISS pour pouvoir être assigné à l'action.

## Comment l'utiliser — Créer une action

{% stepper %}
{% step %}
### Ouvrir le formulaire Créer une action

* Depuis le SIM Board, ouvrir le formulaire **Créer une action**.

<figure><img src=".gitbook/assets/create-action_entry-point-on-the-sim-board.png" alt="Point d'entrée Créer une action sur le SIM Board"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Configurer le contexte SIM

Configurer le contexte SIM :

* **Catégorie** (Sécurité, Qualité, Livraison, Maintenance, Production, Ingénierie) ;
* **Module** (pré-rempli avec la Zone de production du tableau d'origine) ;
* **Ligne**.
* Le **niveau SIM source** et le **niveau SIM cible** sont automatiquement sélectionnés depuis le SIM Board d'origine ; les vérifier avant d'enregistrer car le niveau SIM source devient immuable une fois enregistré.

<figure><img src=".gitbook/assets/create-action_sim-context-bar-category.png" alt="Barre de contexte SIM de Créer une action avec Catégorie"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Saisir le Titre

* Saisir un **Titre** qui identifie le problème (max. 500 caractères).

<figure><img src=".gitbook/assets/create-action_title-field.png" alt="Champ Titre de Créer une action"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Configurer le Statut

* Laisser le **Statut** sur « Nouveau » sauf si le processus SIM local requiert un statut initial différent.

<figure><img src=".gitbook/assets/create-action_status-dropdown.png" alt="Liste déroulante Statut de Créer une action"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Saisir la Description

* Saisir la **Description**. Utiliser le gras, l'italique et les listes pour une meilleure lisibilité.
* Cliquer optionnellement sur **AI Enhance** pour améliorer la clarté ; l'indicateur de qualité fournit un retour en temps réel pendant la saisie.

<figure><img src=".gitbook/assets/create-action_description-with-ai-enhance-and-quality-indicator.png" alt="Description avec AI Enhance et indicateur de qualité"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Définir la Date limite

* Sélectionner une **Date limite** — par défaut aujourd'hui + 7 jours.

<figure><img src=".gitbook/assets/create-action_due-date-picker.png" alt="Sélecteur de Date limite de Créer une action"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Définir Priorité et Gravité

* Définir la **Priorité** (Triviale / Mineure / Majeure / Critique / Bloquante)
* Définir la **Gravité** (Faible / Moyenne / Élevée / Critique)

<figure><img src=".gitbook/assets/create-action_priority-and-severity-dropdowns.png" alt="Listes déroulantes Priorité et Gravité"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Assigner Initiateur, Équipe et Responsable

* Confirmer l'**Initiateur** (pré-rempli avec l'utilisateur actuel ; modifier uniquement si l'on enregistre au nom d'un autre).
* Assigner la responsabilité : au moins l'un entre **Équipe** et **Responsable** doit être configuré pour que l'action ait une partie clairement responsable sur le SIM Board.

<figure><img src=".gitbook/assets/create-action_team-and-owner-assignment.png" alt="Assignation Équipe et Responsable"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enregistrer l'action

* Cliquer sur **Enregistrer l'action**.
* Le bouton vert s'active uniquement lorsque tous les champs obligatoires sont remplis. Une fois enregistrée, l'action est visible sur le SIM Board.

<figure><img src=".gitbook/assets/create-action_save-action-button-active-and-action-visible-on-sim-board.png" alt="Bouton Enregistrer l'action actif et action visible sur le SIM Board"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Comment l'utiliser — Modifier une action

Modifier une action dispose de la **sauvegarde automatique** : chaque champ est confirmé individuellement à la sortie du champ. Il n'y a pas de bouton de sauvegarde global — l'en-tête affiche « Toutes les modifications enregistrées » comme confirmation. Ce comportement permet d'effectuer des mises à jour rapidement pendant la réunion SIM sans interrompre son rythme.

{% stepper %}
{% step %}
### Ouvrir l'action depuis le SIM Board

* Depuis le SIM Board, ouvrir l'action à mettre à jour.

<figure><img src=".gitbook/assets/edit-action_opening-an-action-from-the-sim-board.png" alt="Ouverture d'une action depuis le SIM Board"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Mettre à jour les champs du Panneau de saisie

* Mettre à jour les champs modifiables dans le Panneau de saisie : **Titre, Statut, Description** (avec AI Enhance et indicateur de qualité), **Date limite, Priorité, Gravité, Initiateur, Équipe, Responsable, Pièces jointes**.

<figure><img src=".gitbook/assets/edit-action_entry-panel-with-all-editable-fields.png" alt="Panneau de saisie avec tous les champs modifiables"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Escalader vers un niveau SIM supérieur si nécessaire

* Modifier le **Niveau SIM cible** dans la barre de contexte si l'action doit être escaladée (c'est le seul champ de la barre de contexte qui reste modifiable après la création).

<figure><img src=".gitbook/assets/edit-action_target-tier-dropdown-in-the-context-bar.png" alt="Liste déroulante Niveau SIM cible dans la barre de contexte"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Ajouter ou réviser Solutions et Propositions

* Dans le panneau **Solutions et propositions**, saisir ou coller la solution proposée, ou cliquer sur **AI Suggest** pour générer automatiquement des propositions de solution classées par pertinence.

<figure><img src=".gitbook/assets/edit-action_solutions-proposals-with-ai-suggest.png" alt="Solutions et propositions avec AI Suggest"><figcaption></figcaption></figure>

* Les propositions sont extraites des documents chargés dans la **Source de Connaissance Deep Find**.

<figure><img src=".gitbook/assets/edit-action_solutions-proposals-from-deepfind-document.png" alt="Solutions et propositions extraites de la Source de Connaissance DeepFind"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Ajouter des notes au Journal d'activité

* Ajouter des notes au **Journal d'activité** en bas du panneau ; joindre des fichiers via l'icône trombone si nécessaire. Le Journal d'activité est l'historique complet de l'action sur le SIM Board.

<figure><img src=".gitbook/assets/edit-action_activity-log-with-note-input-and-paperclip.png" alt="Journal d'activité avec saisie de note et trombone"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Définir l'action comme Terminée

* Définir le **Statut** sur « Terminé » uniquement lorsque l'action est genuinement clôturée : « Terminé » verrouille l'ensemble de l'enregistrement.

<figure><img src=".gitbook/assets/edit-action_status-set-to-done-locked-record.png" alt="Statut défini sur Terminé — enregistrement verrouillé"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lecture du résultat

* **Indicateur de qualité** dans la Description — Insuffisant / Acceptable / Bien / Excellent — signale si le texte contient suffisamment d'informations pour être actionnable
* **AI Enhance** réécrit le texte pour plus de clarté professionnelle ; toujours réviser le résultat avant d'enregistrer.
* **AI Suggest** dans Solutions classe les propositions par pourcentage de pertinence par rapport au contenu de la Description.
* Des notifications par e-mail sont envoyées lors d'un changement de statut, d'une nouvelle assignation Équipe/Responsable, d'un avertissement d'échéance à 48 heures et d'actions en retard.

## Conseils et limites connues

{% hint style="info" %}
* Ne pas définir le Statut sur « Terminé » jusqu'à ce que l'action soit genuinement clôturée : il ne peut plus être modifié après.
* Si l'Équipe et le Responsable sont tous deux supprimés, l'enregistrement échoue — toujours conserver au moins l'un des deux assigné.
* La sauvegarde automatique annule le champ en cas d'erreur : vérifier la connexion réseau si un message d'erreur de sauvegarde s'affiche.
* AI Enhance et AI Suggest sont des assistants : le Responsable reste responsable du texte final et de la solution choisie.
* L'escalade entre niveaux SIM s'effectue en modifiant le Niveau SIM cible, pas en créant une nouvelle action — cela préserve l'historique du Journal d'activité du problème original.
{% endhint %}
