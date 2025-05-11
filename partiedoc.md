## Session C: mise en forme des idées

[Retour à la page principale](README.md)

## C.1. Mise en forme des données brutes

### 1.a. Passer d'un texte à un format tabulaire

Soit le texte suivant [lien](https://fr.wikipedia.org/wiki/Agriculture_en_France#Occupation_des_sols_et_du_territoire)

<div class="ex-box">

Construire un tableau à l'aide du prompt suivant:
<ul>
<li>Construire un tableau au format Latex/Excel à partir des données suivantes:</li>
<li>Sélectionner le bloc de texte, le copier, le coller dans le prompt</li>
<li>Copier-coller le tableau dans Excel</li>
</ul>

</div>

### 1.b. Copier-coller de tableaux bruts (uniquement pour les utilisateurs de latex)

Soit le tableau suivant [lien](https://fr.wikipedia.org/wiki/Agriculture_en_France#Productions_agricoles)

<div class="ex-box">

Construire un tableau latex à l'aide du prompt suivant:
<ul>
<li>Construire un tableau au format Latex à partir des données suivantes:</li>
<li>Sélectionner le bloc de texte (=tableau brut), le copier, le coller dans le prompt</li>
</ul>

</div>

### 1.c Lettre de motivation / recommandation

CV (fictif) : [lien](https://github.com/vguigue/tuto-LLM/blob/main/ressources/CV_Vincent_Guigue.pdf)<BR>
Offre de thèse (fictive) : [lien](https://github.com/vguigue/tuto-LLM/blob/main/ressources/sujet.pdf)

<div class="ex-box">

Evidemment, le LLM ne peut pas inventer le contenu!<BR>
Ecrire une lettre de recommandation pour
<ul>
<li>l'étudiant Vincent Guigue</li>
<li>pour une candidature en thèse</li>
<li>comment vous l'avez croisé [UE, projet, stage, ...]</li>
<li>pourquoi vous le recommandez [Sérieux, autonomie, projet remarquable?]</li>
</ul>
Récupérer les éléments qui vous intéressent dans le CV et donner le sujet de thèse au LLM (chatGPT) pour générer la recommandation.

</div>

Pour enrichir la lettre dans un second temps
<div class="ex-box">

<ul>
<li>Quelles sont les qualités recherchées pour ce sujet de thèse?</li>
<li>Quelles sont les éléments critiques pour juger un profil d'étudiant en informatique?</li>
</ul>
➡️ Ajouter les éléments intéressants dans le prompt précédent

</div>

### 1.d Ecrire un paragraphe (introduction) d'article scientifique

La démarche consiste à donner tous les éléments (ou presque) au modèle de langue sous forme de liste de mots-clés ou de bouts de phrases

- Contexte général de la recherche (à donner ou à faire générer) (e.g. l'intéret du machine-learning pour l'analyse des séquences ADN ces dernières années + exemple d'applications)
- Le défi spécifique attaqué dans l'article + les verrous scientifiques actuels / limites des solutions existantes
- Les contributions proposées dans l'article

**Note:** donner ces éléments en français puis demander une génération en anglais

<div class="ex-box">

➡️ Dans l'idéal, prenez un de vos article écrit récemment et tenter de reconstruire une introduction en donnant les bons éléments au modèle de langue

</div>

Sinon, voici une proposition (évidemment très orientée sur le machine learning)

<div class="ex-box">

Idées à faire passer:<BR>
<tt><small> 
tendance actuelle = apport de l'appentissage de représentation non supervisé pour la classification de séries temporelles<BR>
défi = rendre ces approches plus transparentes (échec des approches supervisées); distinguer les types d'explications post-hoc et natives; ne pas perdre en performances (par rapport aux approches SAX)<BR>
contributions = (1) identification des propriétés nécessaire pour l'explicabilité de l'architecture (shift equivariance, décodeur linéaire, conservation des enchainements temporels); (2) proposition d'une architecture basée sur les VQ-VAE; (3) campagne d'expériences sur UCR pour démontrer les performances au niveau de l'état de l'art
</small></tt>
<BR>
Proposition de prompt:
<tt><small> 
Ecrire une introduction d'article scientifique en anglais d'une page détaillant les tendances actuelles du deep learning pour les séries temporelles sur différentes tâches (exemples), puis identifiant les défis actuel du domaine et mettant en avant les contributions. Enrichir les défis par rapport aux contributions
</small></tt>
<BR>
Bonus: Proposer une bibliographie pour chacun des paragraphes

Lien vers l'article original: <a href="https://arxiv.org/abs/2310.16696"> lien </a>
</div>

### 1.e. Résumer, reformuler et améliorer

<div class="ex-box">

Peux tu me faire un résumé très court, en vulgarisant pour un public non scientifique de la page suivante: [https://fr.wikipedia.org/wiki/Loi_binomiale_négative]

<ul>
<li>Donner à chatGPT l'URL entre [] pour lui indiquer la cible, il doit être connecté à internet (cf plus loin)</li>
<li>Indiquer la longueur (e.g. très court)</li>
<li>Indiquer le style (e.g. en vulgarisant pour un public non scientifique)</li>
<li>Option: Illustrer avec un exemple en biologie moléculaire</li>
</ul>

</div>


Autre cas d'usage: reformuler l'une de vos propositions de paragraphe, pour l'améliorer ou la réduire par exemple.

Récupérer un paragraphe: [lien](https://github.com/vguigue/tuto-LLM/blob/main/ressources/paragraph.txt)

<div class="ex-box">

<ul>
<li>Improve the following text</li>
<li>Slightly reduce the length of the following text</li>
</ul>

</div>

### 1.f. Compte rendu de réunion

Mise en forme des notes prises rapidement lors d'une réunion 

- Prendre les notes (non confidentielles) prises lors d'une réunion récente
- ou utiliser le fichier fictif : [lien](https://github.com/vguigue/tuto-LLM/blob/main/ressources/notes.txt)

<div class="ex-box">

Construire un compte rendu de réunion à partir des notes suivantes

<ul>
<li>Spécifier le niveau de langue: soutenu, simple, liste</li>
<li>[opt] Spécifier le format: latex, markdown</li>
</ul>

</div>




## C.2. Exploitation de documents & dialogue documentaire

### 2.a Modèles connectés vs déconnectés

Faire la part des choses entre la mémoire paramétrique et les capacités d'analyse des LLM

<div class="ex-box">

Quelles sont les nouvelles du jour?<BR>
Peux-tu me faire une courte biographie de Vincent Guigue, professeur d'informatique?

<ul>
<li>[connecté] <a href="https://chatgpt.com/"> chatGPT</a> ou <a href="https://www.perplexity.ai/"> perplexity </a></li>
<li>[déconnecté] <a href="https://claude.ai/"> claude</a> ou <a href="https://huggingface.co/chat/"> Huggingface</a> </li>
</ul>

</div>

### 2.b Dialogue avec un document

Charger un document dans NotebookLM [lien](https://notebooklm.google.com/) puis commencer les questions... ($\Rightarrow$ Ajouter une ressource)

OPT 1: le rapport HCERES de l'IPS2: [lien](https://www.hceres.fr/sites/default/files/media/publications/rapports_evaluations/pdf/E2026-EV-0912408Y-DER-ER-DER-PUR260024983-SVE2-IPS2-RF.pdf)

OPT 2: un poly de statistiques (e.g., celui d'A. Guyader): [lien](https://perso.lpsm.paris/~aguyader/files/teaching/M1/PolycopiePartie1.pdf)

<div class="ex-box">

<ul>
<li>Générer un court résumé</li>
<li>Fais moi un quizz de 30 questions pour que le joueur connaisse mieux l'organisation et les thèmes de recherche de l'IPS2</li>
<li>Quelles sont les principales questions scientifiques pour les 5 prochaines années à l'IPS2</li>
<li>L'usage le plus courant de notebookLM consiste à poser des questions très ciblées: e.g. quelle équipe de l'unité IPS2 est prévue d'être arrêtée et quand ?</li>
</ul>
➡️ Le coté multi-lingue fonctionne très bien: posez les questions dans la langue de votre choix!<BR>
➡️ Cliquer sur les liens pour vérifier les citations <BR>
➡️ On peut mettre jusqu'à 50 documents en parallèle dans un projet.
</div>

Note : il faut démarrer un nouveau notebook quand on change de sujet.

Sur un document *Guidelines* pour les projets Horizon: [lien](https://ec.europa.eu/info/funding-tenders/opportunities/docs/2021-2027/horizon/guidance/programme-guide_horizon_en.pdf)

<div class="ex-box">

<ul>
<li>Quelles sont les conditions de base pour monter un projet Horizon?</li>
<li>A partir de combien de partenaires, de quelles natures (académique, industrielle), venant de combien de pays peut-on monter un projet?</li>
</ul>

</div>

Ou avec des documents plus techniques, par exemple, l'article de base sur AlphaFold: [lien](https://www.science.org/doi/epdf/10.1126/science.abm4805) ou une version un peu plus détaillée [lien](https://www.nature.com/articles/s41586-021-03819-2.pdf).

<div class="ex-box">

<ul>
<li> Discuter avec ce document</li>
<li> Résumer et expliquer la méthode</li>
<li> Vous pouvez demander les points forts et les points faibles de l'article... Même lui demander d'en faire une revue</li>
</ul>
➡️  Amusez-vous à générer un dialogue/podcast autour de l'article (bouton en haut à droite)
</div>

Il est amusant de constater que la fonction est aussi présente dans Acrobat Reader (version gratuite) mais limitée à un document.

