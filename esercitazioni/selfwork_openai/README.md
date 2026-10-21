# Selfwork LLM - OpenAI Chat Completion

Un notebook per ogni esercizio della cartella "Esercizi OpenAI":

| File | Esercizio |
|---|---|
| `ex_1_OpenAI_API.ipynb` | Traduzione italiano ⇄ inglese della descrizione di un prodotto |
| `ex_2_OpenAI_API.ipynb` | Estrazione di nome, età e professione da un testo descrittivo |
| `ex_3_OpenAI_API.ipynb` | Riassunto di un articolo in un paragrafo di massimo 255 caratteri |
| `ex_4_OpenAI_API.ipynb` | Descrizione testuale di dati strutturati (dizionario Python) |
| `ex_5_OpenAI_API.ipynb` | Domande di comprensione su un breve testo |

## Avvio

```powershell
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
```

Inserire la propria chiave OpenAI nel file `.env`, poi aprire i notebook selezionando il kernel `.venv`.
