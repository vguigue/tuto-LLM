## Propositions de l'équipe pédagogique d'Ales

[Retour à la page principale](./)

## Analyse du réglement de la scolarité

Dans l'outil NotebookLM:
* lancer l'outil [lien](https://notebooklm.google.com/) + connexion
* nouveau projet
* télécharger les 3 règlements de la scolarité (2024, FISE et FISA) qui sont disponibles ici: [lien](https://github.com/vguigue/tuto-LLM/tree/main/ressources)


Ces tâches s'inscrivent directement dans la logique du RAG. Il est possible de développer des outils spécifiques (par exemple via Ragarenn) ou de faire directement appel à NotebookLM lorsque le nombre de documents à analyser est inférieur à 50.


### Comparaison de versions

<div class="ex-box">


<ul>
<li>Quelles sont les différences entre le règlement FISE et FISA?</li>
</ul>
➡️ Notez les renvois vers les documents originaux
</div>

### Questions spécifiques

Exemple de question spécifique sur le réglement (attention, comme on a mis 3 documents dans le notebook, il faut bien préciser le cadre de la recherche)

<div class="ex-box">

Requête longue:<BR><BR>

Un élève en cursus FISE a tout validé sauf une matière du S9. Il a échoué au rattrapage et d'après le règlement de scolarité il doit repasser l'évaluation avec la promotion suivante (en nov 2025). Il peut s'inscrire en finalisation de cursus pour ça : soit il assiste aussi aux cours et doit payer la moitié des droits d'inscription (qui couvrent de sept. à déc.) soit il ne fait que passer l'examen (ce que je lui ai conseillé).

SA QUESTION : Pourriez-vous me confirmer qu’une fois ce module validé, j’obtiendrai immédiatement le diplôme ? Par ailleurs, serai-je éligible pour effectuer un contrat de professionnalisation ou un stage à partir de septembre 2025 ?

</div>

*LA RÉPONSE ATTENDUE : pour le diplôme il faut que ce soit validé par le jury des études qui suit la constatation qu'il a bien validé (i.e. la correction de l'examen avec mention du prof explicite "module validé". Pour le reste, il ne peut pas faire un stage pour lequel l'école établirait une convention (illégal, travail déguisé...)*

➡️ On notera que la réponse n'est pas parfaite... Mais que la navigation dans le document est plutôt agréable.

<div class="ex-box">
QUESTION ETUDIANT : Est ce que vous sauriez me dire s'il est possible de faire un VIE et que celui ci compte comme PFE ? S'il y a des conditions associées ou autres
choses à savoir. Idéalement, je recherche une expérience professionnelle telle qu'un stage, ou encore un V.I.E. Toutefois, j'aimerais me renseigner sur ce qu'il est possible de faire au cas où je ne trouve pas à temps. Quelles sont toutes les options qui s'offrent à moi en terme d'expérience à l'étranger, qui me permettraient de valider un SIO ?
</div>

*REPONSE PARTIELLE ATTENDUE : oui c'est possible que le VIE se substitut A MOITIE au PFE. En fait deux conventions doivent être établie,  la première concerne les 6 premiers mois du VIE et remplace la convention du PFE. Ensuite, les 6 mois suivants se déroulement "hors école".*


<div class="ex-box">
QUESTION ELEVE : Je me permets de vous contacter pour vous informer que j'ai été accepté pour effectuer un M2 l'année prochaine aux Mines de Saint-Etienne (Master Maths en Actions). Nous avions discuté au début de l'année de mon intention de faire un master dans une autre école d'ingénieur au début des mois de Novembre et de Mai,.

Cette admission en Master  est conditionnée par la validation du M1, qui dépend de la note de stage normalement attribuée au cours du mois de septembre. Après avoir discuté avec deux anciens élèves qui ont été admis en Master l'année dernière, j'ai appris qu'il leur avait été possible de recevoir une note de stage en avance pour commencer leur formation en Master sereinement. Serait-il possible d'envisager la même démarche pour moi, s'il vous plaît?

De plus, pouvez-vous me confirmer que l'admission à ce Master ne compromet pas l'obtention de mon diplôme d'ingénieur? J'ai discuté de ce sujet en début d'année avec James Ollivier, qui m'a assuré que tant que le Master se fait dans un domaine d'ingénierie (ce qui est le cas ici, car il s'agit d'un Master axé sur la Science des Données) et que je paie mes frais de scolarité de troisième année, cela est possible.
</div>

*REPONSE ATTENDUE : Pour la partie administrative, tu es considéré en échange IMT avec Mines Saint Etienne. Tu dois te réinscrire à Alès pour la rentrée de septembre 2024 et tu es assujetti aux droits de scolarité. Tu devras remplir des formalités administrative auprès de Mines St Etienne et il est possible que tu ais des droits de scolarité à payer pour le master.*

<div class="ex-box">
Un étudiant est en mobilité académique. Normalement, à la fin de cette mobilité, il fait un stage (on appelle ça un PFE pour Projet de Fin d'Etudes) est diplômé et peut faire un master derrière s'il le souhaite. Le pb c'est que sa mobilité l'obligerait à rater le master cette année. Or il y a un stage dans le Master. Il demande donc à "mettre en stand by" sa scolarité (il ne lui manque que le PFE) faire le master et prendre un stage qui valide les deux diplômes. 
</div>

*REPONSE:  Le contexte de ta demande : Ton projet est de suivre le M2 du Master Parisien de recherche opérationnelle sur l'année scolaire 2024-2025 à l'issue de ton séjour académique à Hanoi. Pour te diplômer d'IMT Mines Alès, il manque le PFE. Le programme du M2 prévoit un stage de 4 à 6 mois crédité de 20 ECTS. (ce qui est équivalent à notre PFE) <BR> La Proposition : Le stage réalisé dans le cadre du master se substitue au PFE.<BR> Tu suis le Master 2 sur l'année scolaire 2024-2025, IMT Mines Alès suspend ta diplomation.<BR> Tu réalises de stage de fin de master avec une convention du Master mais en demandant au préalable l'accord de ta responsable de département sur le contenu du stage. (il n’y aura pas de convention IMT Mines Alès). Le suivi et l'évaluation de ce stage est faite par le Master. Tu seras diplômé sur la base d'une copie de la convention de stage et de l'attestation de validation du stage de master (Validation des 20 ects) qui devra être fournie par le Master. Cette attestation devra nous parvenir avant début octobre 2025.*

## Approche par compétences

Peut-on exploiter l'outil NotebookLM pour nous aider à projeter des cours dans un référentiel de compétences?
<BR>
Les documents sont disponibles dans [lien](https://github.com/vguigue/tuto-LLM/tree/main/ressources/APC)

L’un des premiers objets à élaborer dans le cadre de cette démarche est une « matrice croisée », qui met en relation les compétences visées par le référentiel et les « acquis d’apprentissages visés » par chaque ECUE au sein d’une UE (= les objectifs d’apprentissage de chaque ECUE). 

A ce stade les syllabus articulent les compétences et les UE. Un travail de formalisation est donc à prévoir à un niveau plus fin (compétences/ECUE), même si ce travail a déjà été initié a minima implicitement pour le globaliser ensuite au niveau de l’UE dans les syllabus.


Pour information, voici la ressource qui va être proposée aux enseignants dans la perspective de travailler à la construction d’une culture commune (enseignants ET élèves) sur la démarche compétences : [La démarche compétences à l'IMT Mines Alès](https://view.genially.com/680202032f83150f653403f6/interactive-content-la-demarche-competences-a-limt-mines-ales) (voir notamment le tableau des notions abordées, accessibles depuis la page 2 « la démarche compétences : trois processus en interrelation » : picto « ampoule »).

<div class="ex-box">
Pour le syllabus TC_5_2 sur l'informatique,  élaborer  une « matrice croisée », qui met en relation les compétences visées par le référentiel et les « acquis d’apprentissages visés » par chaque ECUE au sein d’une UE (= les objectifs d’apprentissage de chaque ECUE).
</div>

Si la réponse n'est pas assez précise, il faut redemander des éléments supplémentaires:

<div class="ex-box">
ATTENTION: il faut commencer par répéter l'ensemble de la question (le système à moins/pas de mémoire sur l'enchainement des questions) 

Je voudrais un tableau séparé pour chaque élément de l'UE:<BR>
TC_5_2-1 Algorithmique et Programmation Objet
<BR>
TC_5_2-2 Réseau
<BR>
TC_5_2-3 Bases de données relationnelles
<BR>
TC_5_2-4 Outils d'analyse
<BR>
➡️ Il est aussi possible de demander un formatage spécifique pour le tableau (latex, markdown, ...)
</div>

Il est aussi possible de jouer avec d'autres outils pour remettre en forme /enrichir les résultats.

<div class="ex-box">

Ne pas hésiter à diversifier les outils et les points de vue:
si on se demande si on n'a rien oublié... Voici un nouveau protocole:

<ul>
<li>Prendre un LLM classique, donner l'intitulé du cours et demander un plan + corriger ce plan pour coller aux attentes de l'équipe pédagogique</li>
<li>Donner uniquement le référentiel au LLM et demander la construction du tableau</li>
</ul>

➡️ Ce n'est pas le même outil, ce ne sera pas la même réponse, pas le même formatage etc...

</div>

### Détecter l'IA dans des textes

Si nous devons apprendre à détecter l'IA dans les travaux des étudiants... Commençons à nous entrainer :)

<div class="ex-box">
Dans les fichiers ci-dessous (2 pep, avec et sans IA), essayer de trouver lequel est l'original et lequel est celui regénérer artificiellement.

<ul>
<li>pep 1, <a href="https://github.com/vguigue/tuto-LLM/blob/main/ressources/PEP/pep1.pdf"> </a>; <a href="https://github.com/vguigue/tuto-LLM/blob/main/ressources/PEP/pep1-w.pdf"> </a></li>

<li>pep 1, <a href="https://github.com/vguigue/tuto-LLM/blob/main/ressources/PEP/pep2-w.pdf"> </a>; <a href="https://github.com/vguigue/tuto-LLM/blob/main/ressources/PEP/pep2.pdf"> </a></li>
</ul>

➡️ L'idée de l'exercice est d'abord de chercher à l'oeil humain puis éventuellement d'utiliser les outils vus dans les exercices précédents.

</div>