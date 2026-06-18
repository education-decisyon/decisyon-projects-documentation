---
icon: star-half-stroke
---

# 2. 5W2H Assisté par IA

### Aperçu général

**5W2H Assisté par IA** est un widget d'évaluation de la qualité qui analyse la complétude et la clarté de l'énoncé d'un problème Kata. Il évalue le texte saisi par l'utilisateur dans les champs État Actuel et État Cible selon le cadre 5W2H — **Qui, Quoi, Pourquoi, Quand, Où, Comment, Combien** — et renvoie un score global de qualité ainsi qu'un retour par dimension. L'objectif est de standardiser les contrôles de qualité entre équipes et sites, en éliminant les révisions incohérentes et subjectives.

<figure><img src=".gitbook/assets/5W2H Cover - Welcome page.png" alt=""><figcaption></figcaption></figure>

## Quand l'utiliser

* Lors de la rédaction de l'**État Actuel** ou de l'**État Cible** d'un nouveau Kata, pour s'assurer que l'énoncé du problème est suffisamment précis et actionnable.
* Lors d'une session de coaching, pour soutenir la conversation avec des éléments tirés directement du texte de l'utilisateur.
* Dans la durée, pour suivre l'évolution de la qualité des énoncés de problèmes entre équipes grâce à un score numérique stable.

## Prérequis

* Le widget **5W2H** doit être activé dans les champs Kata où il doit s'exécuter (généralement État Actuel et État Cible).
* L'utilisateur doit disposer des droits d'édition sur le Kata concerné.

## Comment l'utiliser

{% stepper %}
{% step %}
### Naviguer vers Kata QRCI

* Naviguer vers **Digitized Idea & SIM System → Kata QRCI**. Le tableau de bord affiche tous les Katas existants, filtrables par plage de dates, Statut et KPI. Cliquer sur **Ajouter** (en haut à droite) pour ouvrir le formulaire de création d'un nouveau Kata.

<figure><img src=".gitbook/assets/kata-qrci_dashboard-with-kata-list-and-add-button-highlighted.png" alt="Tableau de bord Kata QRCI avec le bouton Ajouter mis en évidence"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Compléter l'en-tête du Kata

Dans le formulaire d'ajout, configurer les champs de contexte :

* **Zone de production** et **Ligne** (de la hiérarchie d'usine) ;
* **Titre** (un énoncé concis du problème) ;
* **Chef de projet** et **Coach** (tous deux obligatoires) ;
* **Origine** (la catégorie d'origine du problème — ex. Temps d'arrêt, Efficacité, Problèmes de maintenance) et **KPI** (ex. OEE) ;
* **Date de création** est renseignée automatiquement avec la date du jour.

<figure><img src=".gitbook/assets/Kata QRCI — Add form with header fields filled in.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Saisir l'État Actuel (5W2H) et l'Objectif

* Dans les champs **État Actuel** et **Objectif (5W2H)**, décrire la situation actuelle et l'état final souhaité de manière claire et mesurable en suivant le cadre 5W2H : **Qui, Quoi, Pourquoi, Quand, Où, Comment, Combien.**

<figure><img src=".gitbook/assets/5w2h_kata-form-with-current-state-target-state-fields.png" alt="Formulaire Kata avec les champs État Actuel et État Cible"><figcaption></figcaption></figure>

* En cours de saisie, l'indicateur en ligne du widget affiche le score de qualité actuel et le nombre de caractères.

<figure><img src=".gitbook/assets/5w2h_inline-quality-badge-updating-live-as-the-user-types.png" alt="Indicateur de qualité en ligne se mettant à jour en temps réel" width="473"><figcaption></figcaption></figure>

* Cliquer sur l'indicateur en ligne pour ouvrir le popup détaillé.

<figure><img src=".gitbook/assets/5w2h_clicking-the-badge-opens-the-detailed-popup.png" alt="Un clic sur l'indicateur ouvre le popup détaillé" width="563"><figcaption></figcaption></figure>

* Consulter le score circulaire, l'étiquette qualitative et la zone **Focus sur :** suggérée par l'IA.

<figure><img src=".gitbook/assets/5w2h_detailed-popup-with-circular-score-and-focus-on-area.png" alt="Popup détaillé avec score circulaire et zone de focus" width="563"><figcaption></figcaption></figure>

* Ajouter les informations manquantes dans le texte ; le score est mis à jour lors de l'enregistrement du champ.

<figure><img src=".gitbook/assets/5w2h_score-recalculated-after-adding-missing-information.png" alt="Score recalculé après ajout des informations manquantes"><figcaption></figcaption></figure>

* Cliquer sur **Enregistrer** pour créer le Kata.

<figure><img src=".gitbook/assets/kata-qrci_add-form-with-current-status-5w2h-and-target-fields-filled-in.png" alt="Formulaire avec les champs État Actuel et Objectif (5W2H) complétés"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Ouvrir le Kata pour activer le widget 5W2H

* Le nouveau Kata apparaît dans la liste **Kata QRCI**. Ouvrir le Kata : le widget **5W2H Assisté par IA** est maintenant actif dans les champs État Actuel et État Cible et commence à évaluer le texte saisi.

<figure><img src=".gitbook/assets/kata-qrci_newly-created-kata-visible-in-the-list-ready-to-open.png" alt="Nouveau Kata visible dans la liste, prêt à être ouvert"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lecture du résultat

### Les 7 dimensions

Chaque énoncé de problème est évalué selon le même ensemble fixe de dimensions, dans cet ordre : **Qui, Quoi, Pourquoi, Quand, Où, Comment, Combien**.

### Score par dimension

Chaque dimension reçoit une couleur feu tricolore et un score numérique en fonction de la complétude et de la précision avec lesquelles elle est traitée dans le texte.

### Score global de qualité

Le total est la somme des 7 scores par dimension (maximum 14), exprimée en pourcentage de 14 pour obtenir un score de qualité de 0 à 100.

### Tableau récapitulatif

Pour chaque dimension, le widget affiche quatre colonnes :

| Colonne      | Description                                                                   |
| ------------ | ----------------------------------------------------------------------------- |
| Question     | La dimension 5W2H évaluée                                                     |
| Évaluation   | Le score par dimension et la couleur feu tricolore                            |
| Extrait      | La partie du texte utilisée par l'IA pour évaluer la dimension               |
| Suggestion   | Ce qu'il faut ajouter ou clarifier (affiché quand la dimension est absente ou vague) |

## Conseils et limites connues

{% hint style="info" %}
* L'utilisateur garde le contrôle total : les suggestions IA sont indicatives — le texte final est toujours rédigé et enregistré par l'utilisateur
* Le score est calculé sur le texte du champ actuel — rédiger l'État Actuel et l'État Cible indépendamment pour obtenir un retour fiable par champ
* Le widget récompense la précision : dates, noms, lignes, KPIs et quantités mesurables font rapidement monter le score
* La traduction est une fonction de présentation : le score est calculé sur le texte original
* Deux énoncés de problèmes avec le même score global peuvent avoir des profils par dimension très différents — utiliser le tableau récapitulatif, pas seulement le pourcentage global, pour décider quoi améliorer
* 5W2H Assisté par IA est un outil d'orientation : un score durablement faible indique que l'équipe a besoin de coaching sur la formulation des problèmes
{% endhint %}
