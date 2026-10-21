# Selfwork LLM - Ollama Local LLM

Gli esercizi del selfwork OpenAI rifatti con la libreria `ollama` e il metodo `ollama.chat`, usando il modello locale `llama3.2`:

| File | Esercizio |
|---|---|
| `ex_1_Ollama.ipynb` | Traduzione italiano ⇄ inglese della descrizione di un prodotto |
| `ex_2_Ollama.ipynb` | Estrazione di nome, età e professione da un testo descrittivo |
| `ex_3_Ollama.ipynb` | Riassunto di un articolo in un paragrafo di massimo 255 caratteri |
| `ex_4_Ollama.ipynb` | Descrizione testuale di dati strutturati (dizionario Python) |
| `ex_5_Ollama.ipynb` | Domande di comprensione su un breve testo |

## Avvio

Installare Ollama da https://ollama.com e scaricare il modello:

```powershell
ollama pull llama3.2
```

Poi creare l'ambiente virtuale:

```powershell
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

Aprire i notebook selezionando il kernel `.venv`. Non serve nessuna chiave API: il modello gira in locale.
