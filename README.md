# RepoLens

RepoLens is an AI codebase explorer MVP. It gives a repository a visual system map, file-level explanations, dependency signals, generated documentation, and a grounded Q&A surface.

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed by Vite.

## Current scope

This version is a polished, self-contained product prototype. It ships with a realistic `vercel/next.js` demo state and interactive client-side flows:

- GitHub URL validation and demo analysis state
- Overview dashboard with architecture graph, health, codebase stats, and dependencies
- Codebase Time Machine with milestone timeline, change explanations, evidence tags, affected surfaces, and diff preview
- Searchable codebase/file detail view
- Generated documentation view
- Repository Q&A with grounded demo answers and source references

To make analysis live, connect `analyzeRepo` in `src/main.jsx` to a server endpoint that clones/fetches the public repository, parses the tree, builds embeddings, and calls the model provider.
