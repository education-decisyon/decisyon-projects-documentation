---
icon: magnifying-glass
---

# 4. Recherche Approfondie

### Aperçu général

**Recherche Approfondie** est un chatbot IA intégré dans DISS qui permet aux utilisateurs d'interroger une Source de Connaissance configurée — un référentiel de manuels d'usine, procédures, FAQs, politiques, rapports — en langage naturel. Recherche Approfondie analyse les documents qui ont été chargés et synthétise une réponse basée sur leur contenu. Plusieurs documents peuvent être joints à la même conversation pour fournir un contexte plus riche à l'IA.

<figure><img src=".gitbook/assets/DeepFind-Cover Welcome page.png" alt=""><figcaption></figcaption></figure>

## Quand l'utiliser

* Rechercher la procédure pour une intervention spécifique sur un équipement.
* Vérifier les prérequis ou les étapes d'une politique qualité ou sécurité.
* Identifier un code d'erreur apparu sur une machine et trouver les actions correctives recommandées.
* Trouver le bon paragraphe dans un manuel technique volumineux lors d'une investigation Kata.

## Prérequis

* Une Source de Connaissance doit être configurée pour votre site dans DISS.
* Les documents pertinents (manuels, procédures, FAQs, références de codes d'erreur) doivent avoir été chargés dans la Source de Connaissance.
* Recherche Approfondie doit être explicitement activé dans cette Source de Connaissance.

{% hint style="info" %}
Si Recherche Approfondie n'est pas visible dans votre barre d'outils DISS, contactez votre administrateur DISS pour vérifier qu'une Source de Connaissance avec Recherche Approfondie activé a été configurée pour votre site.
{% endhint %}

## Comment l'utiliser

{% stepper %}
{% step %}
### Configurer la Source de Connaissance

* Cette étape est effectuée par un utilisateur ayant le périmètre **administrateur de Source de Connaissance** et doit être réalisée avant que les utilisateurs finaux puissent interroger Recherche Approfondie.

<figure><img src=".gitbook/assets/diss_user-profile-details-with-knowledge-source-administrator-scope-highlighted.png" alt="Profil utilisateur avec le périmètre administrateur de Source de Connaissance mis en évidence"><figcaption></figcaption></figure>

* Cliquer sur l'avatar utilisateur en haut à droite et sélectionner **Sources de Connaissance** dans le menu déroulant. Dans le panneau gauche, cliquer sur **+** pour ouvrir le dialogue de création. Saisir un nom descriptif et cliquer sur **Créer**.

<figure><img src=".gitbook/assets/Knowledge Sources — profile dropdown showing the Knowledge Sources option.png" alt=""><figcaption></figcaption></figure>

* Avec la Source de Connaissance sélectionnée, aller dans l'onglet **Documents** et cliquer sur **Importer un fichier** pour charger les documents pertinents (PDF ou format compatible). Répéter pour chaque fichier supplémentaire.

<figure><img src=".gitbook/assets/knowledge-sources_documents-tab-with-import-file-button-and-uploaded-document-list.png" alt="Onglet Documents avec le bouton Importer un fichier et la liste des documents chargés"><figcaption></figcaption></figure>

* Dans l'onglet **Autorisations**, assigner les organisations et groupes d'utilisateurs autorisés à interroger cette Source de Connaissance.

<figure><img src=".gitbook/assets/knowledge-sources_permissions-tab-with-organisation-and-group-configured.png" alt="Onglet Autorisations avec organisation et groupe configurés"><figcaption></figcaption></figure>

* Dans l'onglet **Agents IA**, activer le sélecteur **Recherche Approfondie AI Assistant** pour connecter cette Source de Connaissance à Recherche Approfondie.

<figure><img src=".gitbook/assets/knowledge-sources_ai-agents-tab-with-deepfind-ai-assistant-enabled.png" alt="Onglet Agents IA avec DeepFind AI Assistant activé"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Ouvrir Recherche Approfondie

* Localiser l'icône **Recherche Approfondie Assistant** dans la barre d'outils DISS et cliquer pour ouvrir l'interface de chat.

<figure><img src=".gitbook/assets/deepfind_assistant-icon-in-the-toolbar.png" alt="Icône DeepFind Assistant dans la barre d'outils"><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/deepfind_chat-interface-opened-empty-state.png" alt="Interface de chat DeepFind ouverte (état vide)"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Poser une question

* Saisir la question en langage naturel — les phrases complètes fonctionnent mieux que les recherches par mots-clés. Pour le dépannage, inclure le code d'erreur et une brève description du symptôme.

<figure><img src=".gitbook/assets/deepfind_typing-a-natural-language-question-with-error-code-example.png" alt="Saisie d'une question en langage naturel avec exemple de code d'erreur"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Lire la réponse et faire un suivi

* Lire la réponse synthétisée. Recherche Approfondie cite le document source et la section à la fin de chaque réponse, pour vérifier la provenance de l'information. Si nécessaire, poser une question de suivi pour affiner ou approfondir la réponse.

<figure><img src=".gitbook/assets/deepfind_synthesised-answer-and-follow-up-turn.png" alt="Réponse synthétisée et tour de suivi"><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Lecture du résultat

Recherche Approfondie synthétise une réponse basée sur les passages les plus pertinents trouvés dans la Source de Connaissance configurée et les documents joints à la conversation. La réponse respecte les politiques d'accès des documents sous-jacents : un utilisateur ne voit que les informations des documents auxquels il a accès.

Lorsque Recherche Approfondie ne peut pas répondre à partir du matériel disponible, il renvoie : _« Je suis désolé, mais je ne peux pas vous aider avec cela car c'est en dehors du périmètre de mes connaissances. »_ Cela signifie qu'aucun document pertinent n'a été trouvé, pas que le sujet n'existe pas.

## Conseils et limites connues

{% hint style="info" %}
* Poser une question à la fois — les questions composées ont tendance à recevoir des réponses partielles.
* Si la réponse est incomplète, reformuler avec des mots-clés différents ou être plus précis sur l'équipement, le processus ou le code d'erreur.
* Si la question est dans le périmètre mais qu'aucune réponse n'est trouvée, consulter l'administrateur DISS pour vérifier que le document pertinent est chargé et Recherche Approfondie activé dans cette Source de Connaissance.
* Recherche Approfondie n'invente pas de contenu : il ne référence que le matériel présent dans la Source de Connaissance configurée ou les documents joints.
{% endhint %}
