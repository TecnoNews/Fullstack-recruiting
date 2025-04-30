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
- **Database**: PostgreSQL (struttura dati già fornita)

---

## 📦 Base Dati fornita

Ti verranno forniti:

- Un file `.sql` di esempio con:
  - 10 quiz logici precompilati
  - 3 utenti fittizi
- Tabelle:
  - `users (id, email, nickname)`
  - `quizzes (id, question, type, options, correct_answer, explanation)`
  - `answers (id, user_id, quiz_id, user_answer, is_correct, created_at)`

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

- Capacità di ragionare sulle logiche applicative
- Strutturazione chiara del codice (frontend e backend)
- Scelta di pattern e organizzazione del flusso dati
- Uso corretto di CSR/SSR in Next.js
- Gestione API sicura e pulita (NestJS)

---

## ✨ Bonus (non obbligatorio)

- Scrivere qualche test base (es. per le API)
- UI semplice ma curata (es. uso di TailwindCSS o simili)

---

## 📅 Consegna

- Repo GitHub privata o archivio ZIP.
- Deve includere un file `README.md` con:
  - Istruzioni per avviare il progetto
  - Descrizione di eventuali scelte progettuali
