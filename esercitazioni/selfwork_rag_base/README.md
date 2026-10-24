# Selfwork RAG Base

Esempio base di RAG (Retrieval Augmented Generation) con ChromaDB e OpenAI.

1. I curriculum in `resumes/` vengono letti e divisi in paragrafi (separatore `### `).
2. Ogni paragrafo viene trasformato in embedding con `text-embedding-3-small` e salvato in una collection ChromaDB, insieme al nome del file e ai dati del candidato.
3. Data la richiesta dell'utente, ChromaDB restituisce il paragrafo più simile.
4. Il paragrafo trovato viene inserito come contesto nel prompt e `gpt-4o-mini` indica il candidato più adatto, motivando la scelta.

## Avvio

```powershell
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
```

Inserire la propria chiave OpenAI nel file `.env`, poi eseguire lo script dalla cartella `selfwork_rag_base`:

```powershell
python rag_base.py
```
