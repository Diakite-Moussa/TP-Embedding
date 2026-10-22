# 🧠 Travaux Pratiques : Les Embeddings avec LangChain & Ollama

**Université Mundiapolis Casablanca**  
**Enseignant :** Pr. Habib AYAD  
**Classe :** 3ACINF DATA  
**Année Universitaire :** 2026 – 2027  

---

## 📄 Rapport Interactif & Version PDF

Ce dépôt contient le code source complet et les corrections détaillées des **exercices 1 à 5** du TP.

👉 **Consulter le rapport interactif en ligne :**  
Une page web dédiée avec les codes sources, les sorties console réelles, les analyses critiques et un bouton d'export PDF en 1 clic est disponible directement via **GitHub Pages** :  
`https://<votre-nom-d-utilisateur>.github.io/<nom-du-repo>/` *(ou en ouvrant directement `index.html`)*.

---

## 🎯 Contenu du TP & Exercices Traités

| Exercice | Thématique | Objectif |
|---|---|---|
| **Exercice 1** | **Synonymes & Paraphrases** | Analyse de la similarité cosinus sur des paraphrases vs paires polysémiques (« avocat »). |
| **Exercice 2** | **Propriétés Multilingues** | Alignement sémantique inter-langues (FR, EN, AR) et étude du biais linguistique. |
| **Exercice 3** | **Impact de la Dimension** | Trade-off entre compression vectorielle (64, 256, 768 dims) et stabilité du ranking. |
| **Exercice 4** | **Mini FAQ RAG Intelligente** | Indexation de Q/R dans `InMemoryVectorStore` avec seuil de confiance et rejet hors-sujet. |
| **Exercice 5** | **Classification Zero-Shot** | Attribution thématique non supervisée et pistes d'amélioration par prompting d'étiquettes. |

---

## 🚀 Installation & Exécution Locale

### 1. Prérequis
- **Python 3.10+** (ou `uv`)
- **Ollama** avec le modèle d'embedding local :
  ```bash
  ollama pull nomic-embed-text
  ```

### 2. Installation des dépendances
```bash
pip install -r requirements.txt
# ou avec uv :
uv sync
```

### 3. Lancer le Notebook Jupyter
```bash
jupyter notebook TP_Embeddings_LangChain_OpenAI_mundia.ipynb
```

---

## 🌐 Déploiement sur GitHub Pages (pour donner le lien au professeur)

1. **Initialiser et pousser sur GitHub :**
   ```bash
   git add .
   git commit -m "feat: ajout du rapport complet index.html et des exercices 1 a 5"
   git branch -M main
   git remote add origin https://github.com/<votre-username>/<nom-du-repo>.git
   git push -u origin main
   ```

2. **Activer GitHub Pages :**
   - Allez sur votre dépôt GitHub dans **Settings** > **Pages** (dans le menu de gauche).
   - Sous **Build and deployment** > **Branch** : sélectionnez `main` (ou `master`) et le dossier `/ (root)`.
   - Cliquez sur **Save**.
   - Après 1 à 2 minutes, GitHub génère l'URL publique de la page :  
     `https://<votre-username>.github.io/<nom-du-repo>/`
   - Il vous suffit de copier et transmettre ce lien à votre professeur !
