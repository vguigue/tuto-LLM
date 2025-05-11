
Nous allons voir les usages *recherche*, notamment bibliographique et écriture d'article puis des usages plus pédagogiques sur la rédaction de cours, la création d'exercice.

## B.1. Bibliographie

C'est un des usages controversé: on a beaucoup cité la bibliographie comme la chose à NE PAS faire avec un LLM... Tentons quelques expériences.

### 1.a Bibliographie et hallucination

Une hallucination est un résultat faux... mais obtenu en maximisant la vraisemblance du texte. Transposé dans le domaine de la bibliographie, cela se traduit par des référénces qui n'existent pas... Mais qui sont très crédibles!

<div class="ex-box">
<ul>
<li> Je voudrais une bibliographie sur la technique CRISPR-CAS9 [remplacer par le terme technique de votre choix]</li>
</ul>

➡️ par exemple en sélectionnant le modèle  <tt>meta-llama/Llama-3.3-70B-Instruct</tt> dans l'interface Huggingface/ragarenn <BR> 
Tester les différentes références: si >90% sont bonnes, que faut-il en conclure?
<BR>
➡️ plus les références sont classiques (=beaucoup citées), plus elles sont correctes... Mais il faudra toujours les vérifier !
<BR>
➡️ Ca vaut le coup de refaire l'expérience sur un domaine plus pointu (moins général) pour avoir plus d'hallucinations... Il faut aussi différentier le mode LLM (mémoire paramétrique) et le mode RAG (sur chatGPT par exemple).
</div>

<div class="ex-box">
Générer une bibliographie sur la technique CRISPR-Cas9: distinguer les références qui précèdent cette technique, les références qui fondent CRISPR-Cas9 et les avancées récentes sur ces architectures
<ul>
<li>Remplacer le CRISPR-Cas9 par ce que vous voulez</li>

</ul>

➡️ Encore et toujours une histoire de véracité: il faut vérifier que les références existent... Et sont bien pertinentes!
</div>

### 1.b Usage en bibliographie : identifier une source primaire

Retrouver une source primaire sur [Scholar](https://scholar.google.com) n'est pas simple... Sur des techniques très connues (CRISPR-Cas9 en biologie moléculaire, les SVM, VAE ou Transformer en IA, ...)


<div class="ex-box">
<ul>
<li> Quelle est la référence biblio primaire de CRISPR-Cas9? [remplacer par une technologie très citée dans votre domaine]</li>

</ul>

</div>

### 1.c Usage en bibliographie : structurer la bibliographie

<div class="ex-box">
<ul>
<li> Je veux faire une bibliographie sur l'usage des données textuelles dans les systèmes de recommandation: peux-tu me proposer une structuration avec différents usages et quelques références</li>

</ul>

➡️ plus les références sont classiques (=beaucoup citées), plus elles sont correctes... Mais il faudra toujours les vérifier !

</div>


## B.2. Création de contenus : plan de cours / brainstorming / exercices

### 2.a Plan de cours

L'enjeu est de trouver rapidement un plan... De vérifier qu'on n'a rien oublié d'important... Puis de pousser plus loin pour faire sortir des idées originales.

<div class="ex-box">

Je veux construire le plan d'un cours sur XXX [e.g. l'Intelligence Artificielle]

<ul>
<li>Proposer un plan de cours en 10 parties</li>
<li>Renouveler l'opération sur les items pertinents pour obtenir des détails (ou demander dès le début des sous-parties)</li>
</ul>

➡️ Juger ce qui est (1) pertinent mais évident, (2) pertienent et original, (3) discutable ou faux
</div>


### 2.b Exercices & quizz

Et pour générer un quizz (très à la mode pour des évaluations mieux réparties et robustes à chatGPT)...

<div class="ex-box">

Je suis en train de faire un cours sur [XXX détaillé] (e.g. les modèles de deep learning pour l'image (CNN, ViT) avec des étudiants en informatique de niveau Master 2)\\ Peux-tu me générer un quizz de 4 questions sur ce thème?
<ul>
<li> Demander 10 ou 20 questions pour avoir plus de choix (certaines questions seront plus pertinentes que d'autres !)</li>
<li> OPT: Demander une génération en latex (si vous utilisez ce format)</li>
<li> Comparer avec un des exercices suivant où on fera la même chose... En donnant le poly de cours comme base</li>
</ul>

</div>

### 2.c Rédaction/gestion de projets

Quelques exemples:

<div class="ex-box">

Générer un texte d'un demi page sur les usages de l'IA dans votre métier/votre équipe de recherche en mode SWOT (Strengths, Weaknesses, Opportunities, Threats). Ajouter des informations sur votre équipe sous forme de liste de mots clés. <BR>

On peut envisager différentes options:
<ul>
<li>Ce texte a vocation a être publié sur la page web de votre équipe</li>
<li>Ce texte est une réponse à appel à projet (AAP), il doit être crédible tout en mettant en avant votre équipe pour obtenir des financements</li>
</ul>
</div>


<div class="ex-box">

Je veux déposer un projet ANR sur le développement de systèmes de recommandation en nutrition [remplacer par votre sujet de prédilection!].

<ul>
<li>Quels sont les enjeux de ce type de systèmes? Générer des arguments explicant l'intérêt de ces systèmes (sur le plan de la santé, des économies, de la souveraineté alimentaire, ...) [on peut décomposer en plusieurs questions]</li>
<li>Structurer une bibliographie pour ce projet en distinguant les types d'applications et les modèles associés.</li>
<li>Quelles sont les sources de données disponibles pour apprendre ces systèmes de recommandation?</li>
</ul>
</div>

<div class="ex-box">

Je veux organiser un séminaire sur les nouvelles techniques autour des petits ARN pour les plantes de 2 jours avec des inscriptions gratuites pour les orateurs et payantes pour les participants dans le cadre d'une université francaise. Quelles sont les grandes étapes? Par ou commencer?

<ul>
<li>Ne pas hésiter à demander des outils pour certaines étapes (e.g. sélection des aarticles)</li>
<li>Auprès de qui rechercher un budget? Comment procéder? Ecrire les lettres de demande</li>
</ul>
</div>

## B.3. Dans la peau d'un étudiant

The good, the bad, the ugly: les LLM ont de multiples visages qui nous imposent de repenser notre pédagogie.

### 4.a Poser des questions sur un énoncé
Le LLM est une sorte de prof disponible 24/7 à qui on peut poser toutes les questions sans avoir peur...

<div class="ex-box">

<ul>
<li> Dans le cours sur les tris de listes, peux tu m'expliquer le tri par bulle? (OPT : demander le code python, ajouter des commentaires, générer des exemples de tests pour valider ma solution...)</li>
<li> Peux-tu me donner toutes les étapes pour calculer la représentation binaire 32 bits de 34.5 en virgule flottante?</li>
</ul>
➡️ Evidemment, on peut/doit rebondir sur les réponses avec de nouvelles questions
<BR>
➡️ En tant qu'enseignant, on voit rapidement que l'usage est assez différent de wikipedia

</div>

➡️ Note importante: le prof reste une personne importante et incontournable pour de nombreux aspects !!

### 4.b Générer des exercices pour les révisions

<div class="ex-box">

<ul>
<li> Quelles sont les questions les plus classiques dans un cours de physique sur la refraction?</li>
<li> Dans le cadre d'un cours de L2 informatiques sur l'algorithmique, nous avons une interrogation sur le tri des listes, quelles sont les questions les plus probables?</li>
</ul>
➡️ Evidemment, on peut demander des précisions et/ou des réponses pour vérifier
</div>



### 4.c Traiter directement un énoncé

L'usage classique des étudiants (peu apprécié par le corps enseignant).
Soit le fichier d'examen suivant [lien](https://github.com/vguigue/tuto-LLM/blob/main/ressources/quizz.pdf).

<div class="ex-box">
En fournissant le fichier (ou son URL)
<ul>
<li> Donner les réponses des questions de cet examen de machine learning</li>
</ul>
➡️ N'hésitez pas à faire le test avec vos examens... 
</div>

### 4.d Détecter les tricheurs

Il existe des outils de détection (statistique) des textes générés par des IA, par exemple [GPTzero](https://gptzero.me/); [zeroGPT](https://www.zerogpt.com/); [lien](https://copyleaks.com/ai-content-detector)

<div class="ex-box">
Soit l'énoncé jouet [remplacable par ce que vous voulez]:<BR> Expliquer brièvement le fonctionnement d'un algorithme de classification (2 classes) Naive Bayes basé sur une modélisation de Bernoulli.

<ul>
<li> Donner l'énoncé à un LLM et copier la réponse</li>
<li> Aller sur GPT Zero et coller dans la boite</li>
<li> Que se passe-t-il si vous demandez au LLM de reformuler sa réponse (ou que vous le faites à la main):<BR> Reformuler la réponse sans les formules et avec des phrases plus simple tout en gardant les mots clés techniques. Ajouter quelques fautes d'orthographes.</li>
<li> Que se passe-t-il lorsque vous donnez un paragraphe de wikipedia? Par exemple tiré de <a href="https://fr.wikipedia.org/wiki/Wikipédia:Accueil_principal">lien<a></li>
</ul>
➡️ Comment analyser ces chiffres? Comment s'en servir?
</div>


## B.5. Analyse automatique de dossier (e.g. MonMaster)

La réforme *TrouverMonMaster*, discutable dans ses hypothèses, sa mise en oeuvre et ses conséquences, nous pousse à trouver des solutions originales pour analyser les lettres de motivation...

### 5.a Quelques questions sur une lettre de motivation


<div class="ex-box">
A partir du fichier <a href="https://github.com/vguigue/tuto-LLM/blob/main/ressources/notes.txt">lien</a>, l'idée est de poser des questions pour remplir un formulaire.

Voici des exemples de questions

<ul>
<li> Analyser la lettre suivante en répondant à la liste de questions</li>
<li> Le candidat demande-t-il le master MIND?</li>
<li> Le candidat a-t-il fait des projets en IA? Donner les titres.</li>
<li> Le candidat a-t-il fait des stages en IA en entreprise? En laboratoire académique?</li>
<li> Demander les résultats en JSON, analyser un pdf...</li>
</ul>
➡️ Il faut imaginer l'usage de LLM locaux <a href="https://ollama.com">type ollama</a> et de bibliothèque de lecture de pdf <a href="https://pypdf.readthedocs.io">type pypdf</a> dans des outils comme <a href="https://www.langchain.com/">langchain</a> ... Avec un LLM pour vous guider, vous pouvez développer un outil rapidement.
</div>



### 5.b Analyser des bulletins de notes / OCR

Les techniques d'OCR (extraction de textes) ont significativement progressé avec les LLM. On pourrait envisager de nouvelles applications sur les candidatures.



<div class="ex-box">
Dans le document suivant: <a href="https://github.com/vguigue/tuto-LLM/blob/main/ressources/couverture.jpeg">lien</a>

<ul>
<li> Analyser l'image suivante pour trouver l'éditeur et l'année de publication</li>
</ul>
➡️ Les derniers modèles Llama sont capables de réaliser ces opérations localement (=sur votre -gros- ordinateur) <BR>
➡️ Sur un bulletin de notes, il faut retrouver l'année d'étude, regrouper les matières par domaines (les noms variants d'une licence à l'autre) puis remplir un formulaire...<BR>
➡️ Plus on pose des questions précises, plus on guide l'extraction qui gagne en performance.
</div>


## B.6.  Générations amusantes

<div class="ex-box">
Trouver un acronyme pour un projet de recherche sur les petits ARN: l'idée est d'optimiser la réponse des plantes aux stress environnementaux avec de l'IA

<ul>
<li>On peut spécifier la langue (le LLM part vers l'anglais ou le franglais par défaut)</li>

</ul>
</div>

<div class="ex-box">

Rédiger un poème sur les petits ARN, la réponse des plantes aux stress environnementaux, les perspectives d'utilisation de l'IA pour le futur. Les rimes seront croisées.
<ul>
<li>On peut préciser la langue ou rajouter des élements dans le prompt ou dans les questions suivantes</li>
<li>Si vous voulez ensuite générer de l'audio, différents outils existent: e.g. <a href="https://elevenlabs.io/app/speech-synthesis/text-to-speech"> lien </a> </li>
</ul>

Note: le test avec chatGPT est très concluant!
</div>