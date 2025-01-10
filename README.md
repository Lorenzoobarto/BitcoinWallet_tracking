# Welcome to BitAlert

BitAlert è un'applicazione web progettata per tracciare e analizzare transazioni di Bitcoin, fornire avvisi email per nuove attività su wallet Bitcoin e generare report dettagliati in formato Word ed Excel.

## Struttura del Progetto
**BitAlert.py:** File principale che contiene la logica dell'applicazione e gli endpoint Flask.

  - **Cartella static:** Contiene file statici come immagini e grafici generati.
    
  - **Cartella templates:** Contiene file HTML per il rendering delle pagine web:
     - **home.html:** Pagina iniziale dell'applicazione.
     - **index.html:** Interfaccia per tracciare le transazioni di un wallet Bitcoin e scaricare i report.
     - **page_two.html:** Pagina per avviare gli avvisi email su nuove transazioni.
       
  - **File di template aggiuntivi:**
     - **template.docx:** Template per i report in formato Word.
     - **template.xlsx:** Template per i report in formato Excel.

## Funzionalità Principali
Una volta avviato BitAlert, nella prima pagina, si avrà l'opzione di scegliere una delle due funzionalità del progetto.

**TRACCIAMENTO WALLET**
- Inserisci un indirizzo Bitcoin per ottenere le transazioni recenti.
- Visualizza grafici per flussi in entrata e uscita.
- Modifica i grafici e la tabella delle transazioni tramite i filtri: Direzione (entrata, uscita) - Intervalli di prezzo - Date specifiche - Stato di conferma (pending, confermato)
- Scarica report in formato Word o Excel.

**ALERT SU TRANSAZIONI**
- Inserisci un wallet valido e un'email su cui vuoi ricevere le notifiche sulle nuove transazioni confermate.

## Setup del Progetto

**PREREQUISITI**
- Python 3.8 o superiore.
- Librerie richieste (installabili con pip):
```bash
pip install flask matplotlib requests python-docx openpyxl
```
**CONFIGURAZIONE**
1. Configura il file **BitAlert.py** con le tue credenziali email per inviare notifiche:
```bash
EMAIL_ADDRESS = "tuo_email@gmail.com"
EMAIL_PASSWORD = "tua_password_app"
```
2. Assicurati che i file **template.docx** e **template.xlsx** siano nella directory corretta.
