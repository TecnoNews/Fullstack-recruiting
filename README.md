# Test Tecnico Fullstack – Progetto "Gestione Quiz Logici"

## 🎯 Obiettivo

Realizzare un'app che permetta:

- Agli **utenti registrati** di rispondere a quiz logici (area privata CSR con React).
- A chiunque di **vedere** la classifica e i dettagli dei quiz (area pubblica SSR).

---

## ⚙️ Stack obbligatorio

- **Frontend**: Next.js
  - **CSR**: Dashboard privata utente + risposta ai quiz
  - **SSR**: Pagine pubbliche di classifica e dettaglio quiz
- **Backend**: NestJS
- **Database**: PostgreSQL

---

## 📦 Dati iniziali

I seguenti dati possono essere inseriti a mano nel database o importati tramite script. Per semplificare, non è richiesto un backoffice.

### 👤 Utenti fittizi

| ID | Email              | Nickname |
|----|--------------------|----------|
| 1  | alice@example.com  | Alice    |
| 2  | bob@example.com    | Bob      |
| 3  | charlie@example.com| Charlie  |

### 🧠 Quiz logici (a risposta multipla)

Ogni quiz ha:
- Una domanda
- Quattro opzioni
- Una risposta corretta
- Una spiegazione

#### Quiz 1
**Domanda**: Un contadino ha 17 pecore. Tutte tranne 9 scappano. Quante rimangono?  
**Opzioni**: 9, 8, 17, 0  
**Risposta corretta**: 9  
**Spiegazione**: Se tutte tranne 9 scappano, allora 9 restano nel recinto.

---

#### Quiz 2
**Domanda**: Alcuni mesi hanno 30 giorni, altri 31. Quanti ne hanno 28?  
**Opzioni**: 1, 12, 2, Solo febbraio  
**Risposta corretta**: 12  
**Spiegazione**: Tutti i mesi hanno almeno 28 giorni.

---

#### Quiz 3
**Domanda**: Quanti animali di ogni specie Mosè portò sull'arca?  
**Opzioni**: 2, 1, Nessuno, Non era Mosè  
**Risposta corretta**: Non era Mosè  
**Spiegazione**: Fu Noè, non Mosè.

---

#### Quiz 4
**Domanda**: Se impieghi 5 minuti per tagliare 5 tronchi, quanto impieghi per tagliarne 100?  
**Opzioni**: 100, 50, 105, 100 minuti  
**Risposta corretta**: 100  
**Spiegazione**: Ogni tronco richiede 1 minuto.

---

#### Quiz 5
**Domanda**: Quale parola è sempre scritta in modo errato nel dizionario?  
**Opzioni**: Errato, Sbagliato, Mai, Corretto  
**Risposta corretta**: Errato  
**Spiegazione**: La parola "errato" è letteralmente scritta come "errato".

---

#### Quiz 6
**Domanda**: Un aereo si schianta sul confine tra Italia e Francia. Dove seppelliscono i sopravvissuti?  
**Opzioni**: Francia, Italia, Entrambi, Da nessuna parte  
**Risposta corretta**: Da nessuna parte  
**Spiegazione**: I sopravvissuti non si seppelliscono.

---

#### Quiz 7
**Domanda**: Se un treno elettrico va verso sud e tira vento da nord, dove va il fumo?  
**Opzioni**: Sud, Nord, Est, Da nessuna parte  
**Risposta corretta**: Da nessuna parte  
**Spiegazione**: Un treno elettrico non fa fumo.

---

#### Quiz 8
**Domanda**: Quante lettere ha l'alfabeto?  
**Opzioni**: 21, 26, 11, Quante ne servono  
**Risposta corretta**: 11  
**Spiegazione**: La frase "l'alfabeto" ha 11 lettere.

---

#### Quiz 9
**Domanda**: Puoi sollevare un elefante con una sola mano?  
**Opzioni**: Sì, No, Solo da piccolo, Nessuno ha mani così forti  
**Risposta corretta**: Nessuno ha mani così forti  
**Spiegazione**: Nessuno ha una sola mano così forte.

---

#### Quiz 10
**Domanda**: Cosa pesa di più: un chilo di ferro o un chilo di piume?  
**Opzioni**: Ferro, Piume, Sono uguali, Dipende  
**Risposta corretta**: Sono uguali  
**Spiegazione**: Entrambi pesano un chilo.

---

## 🧩 Funzionalità richieste

### 1. Autenticazione (mock)

- Login/signup senza sistema reale di email/password (puoi simulare login via nickname).

### 2. Area Privata - CSR

- Elenco quiz disponibili.
- Risposta ai quiz (una volta sola per quiz).
- Visualizzazione dei propri risultati personali.

### 3. Area Pubblica - SSR

- Pagina **classifica pubblica** (top utenti per numero di risposte corrette).
- Pagina **dettaglio quiz**:
  - Domanda
  - Spiegazione logica
  - Percentuale utenti che hanno risposto correttamente

---

## 🧠 Focus di valutazione

- Capacità di ragionamento logico
- Architettura chiara frontend/backend
- Uso corretto di CSR/SSR in Next.js
- API ben strutturate e sicure in NestJS

---

## ✨ Bonus (non obbligatorio)

- Scrivere qualche test base (es. per le API)
- UI curata e moderna (es. uso TailwindCSS)

---

## 📅 Consegna

- Repo GitHub privata o archivio ZIP
- Include un file `README.md` con:
  - Istruzioni per avvio
  - Note su eventuali scelte architetturali

---

## 📝 Nota finale

Qualsiasi aggiunta o miglioramento che ritieni utile – sia tecnico, funzionale o estetico – è assolutamente ben accetto. Usa questo test anche come occasione per mostrare il tuo modo di ragionare, proporre soluzioni e organizzare un piccolo progetto end-to-end.

