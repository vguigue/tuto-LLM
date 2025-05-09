
## Session 1: matin

Première série d'exercice pour prendre en main les LLM, découvrir de nouveaux usages et prendre du recul par rapport aux réponses.

## 1. En pratique: se lancer avec un LLM


### 1.a. Préliminaire: comprendre l'unité de base des LLM: le token

Lien: [Tokenizer Playground](https://huggingface.co/spaces/Xenova/the-tokenizer-playground)

<div class="ex-box">
Mettre en évidence la gestion des langues en tokenisant:

<ul>
<li> Je ne suis pas très content </li>
<li> I'm so disappointed </li>
<li> Vous pouvez copier-coller des morceau de wikipedia pour une vision plus large: <a href="https://fr.wikipedia.org/">lien fr </a>; <a href="https://en.wikipedia.org/">lien eng </a> 
</li>
</ul>


➡️ Avec chatGPT (multi-lingue) ou BERT (anglophone)
</div>

### 1.b. Les LLMs sur les lesquels nous allons travailler

<div class="ex-box">
➡️ Vous pouvez ouvrir les 7 premiers dans des onglets: nous allons jouer avec dans la suite
</div>

- **chatGPT**: le modèle à l'origine de l'ouverture des LLM au grand public [lien](https://chatgpt.com/)
    - lien avec internet
    - possibilité de générer des images
- **huggingface**: directement lié à la bibliothèque qu'utilise les chercheurs [lien](https://huggingface.co/chat/)
    - tester différents modèles (plus) ouverts
    - modèles de raisonnement
- **perplexity**: une alternative à chatGPT [lien](https://www.perplexity.ai/)
- **mistal**: le chat, réputé champion français [lien](https://chat.mistral.ai/)

Les sites de comparaison directe de modèles:

- **Site gouvernemental**: [lien](https://www.comparia.beta.gouv.fr)
    - etimation de la consommation des LLMs (en plus de la comparaison des résultats)
- **lmarena**: le site historique de benchmark humain [lien](https://lmarena.ai) 

Les LLM en mode RAG, pour dialoguer avec des documents:

- **NotebookLM**: [lien](https://notebooklm.google.com/)

### 1.c. Et ceux, intéressants, que vous pourrez tester après la session de formation

- **Claude**: le modèle d'Anthropic [lien](https://claude.ai/)
    - beaucoup de recherche pour epxliquer les résultats... Mais pas encore visible pour le grand public
- **ollama**: pour faire tourner des LLMs en local sur votre ordinateur [lien](https://ollama.com/)
    - Télécharger, lancer, ouvrir une console, lancer un modèle dans la console (attention, le téléchargement du LLM a lien à ce moemnet là).
    - Idéal pour les données sensibles, les chaines de traitements de pdf ou autres
- **Grok**: pour voir la différence avec des modèles libertariens [lien](https://grok.com/chat)
- **aristote**: pour un dialogue sécurisé (accès avec des identifiant académique) [lien](https://chat.aristote.education)
