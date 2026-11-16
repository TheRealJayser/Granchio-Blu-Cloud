# Granchio Blu (con accesso Google)

Web app per registrare il pescato di granchio blu: giorno, chili e prezzo al chilo, con totali dell'anno e confronto con gli anni precedenti.

Questa versione aggiunge **l'accesso con Google** e salva i dati online, così non si perdono se si rompe il telefono e ognuno (papà, amici) ha il proprio registro. È nata dalla versione 2.3 di [Granchio-Blu-App-Tracker](https://github.com/TheRealJayser/Granchio-Blu-App-Tracker).

**App online:** https://granchio-blu-cloud.netlify.app

## Come si usa

1. Apri il link dal telefono e premi **Accedi con Google**.
2. Su iPhone: *Condividi → Aggiungi alla schermata Home*. Su Android: menu ⋮ → *Installa app*.
3. Inserisci il pescato con il **+**. Senza campo va bene lo stesso: i dati partono appena torna la rete.

Per portare i dati dalla vecchia app: nella vecchia app *menu → Backup → Copia*, poi nella nuova *menu → Backup → Ripristina*, incolla e premi **Importa**. Oppure importa di nuovo il file Excel dei conferimenti.

## Come è fatta

- `index.html`: tutta l'app (HTML, stile e codice).
- **Firebase** (progetto `granchio-blu`, piano gratuito Spark):
  - *Authentication* con Google;
  - *Cloud Firestore* (Milano, `europe-west8`), dati in `users/{uid}/uscite/{AAAA-MM-GG}` con `d`, `kg`, `p`.
- `firestore.rules`: copia delle regole di sicurezza pubblicate (ognuno legge e scrive solo i propri dati). Se le cambi, ripubblicale dalla console Firebase.
- `_redirects`: su Netlify l'accesso Google passa dallo stesso dominio dell'app, altrimenti Safari su iPhone lo blocca.
- `sw.js`: fa aprire l'app anche senza connessione.

Pubblicata su Netlify, collegata a questa repository: ogni modifica su `main` va online da sola. Le novità sono in [CHANGELOG.md](CHANGELOG.md).
