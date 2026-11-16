# Novità

Tutti gli aggiornamenti dell'app Granchio Blu (versione con accesso Google), dal più recente.

## Versione 3.3 — 16 novembre 2026

### Aggiunto
- **Grafico di confronto** nella sezione *Anni*: i chili accumulati dall'inizio dell'anno, una linea per anno. Scorrendo col dito sul grafico si leggono i valori di ogni anno a quella data.

### Corretto
- **Esportazione in Excel:** non funzionava. Ora il file viene creato direttamente dall'app, anche senza rete, e contiene quattro colonne: giorno, chili, prezzo €/kg e incasso (le ultime due solo nei giorni con il prezzo), più la riga del totale.
- I numeri nei riquadri di riepilogo (*Oggi*, *Uscite*) ora sono centrati.

## Versione 3.2 — 16 novembre 2026

### Aggiunto
- **Questa settimana** nella Home: i chili della settimana in corso confrontati con la settimana scorsa (anche "a pari giorno", cioè fino allo stesso giorno della settimana) e con la stessa settimana dell'anno prima.
- **Vista Settimane** nella sezione *Uscite*: accanto a *Giorni* si può scegliere *Settimane* per vedere ogni settimana dell'anno con chili, uscite, media, incasso e la differenza rispetto alla settimana prima. Le settimane vanno da lunedì a domenica.

### Modificato
- Nel tema scuro torna lo **sfondo blu scuro** della prima versione, al posto del nero.

## Versione 3.1 — 16 novembre 2026

Nuova grafica in stile iOS, con animazioni e personalizzazione.

### Aggiunto
- **Barra in basso** con quattro sezioni: *Home*, *Uscite*, *Anni* e *Impostazioni*. Si cambia sezione toccando la barra oppure **scorrendo col dito** a destra e a sinistra. Il **+** per inserire il pescato sta accanto alla barra.
- **Personalizzazione** in *Impostazioni → Aspetto*: tema automatico, chiaro o scuro, e sei colori per l'app (blu granchio, laguna, alga, corallo, viola, ardesia).
- **Animazioni:** il totale dell'anno conta fino al valore, le barre crescono, le righe entrano una dopo l'altra, l'uscita appena salvata si illumina, gli avvisi scendono dall'alto.
- Nella sezione *Uscite* gli anni si scelgono con i pulsanti in alto e c'è il riepilogo dell'anno (chili, uscite, media).
- Nella sezione *Anni* ogni anno ha la sua barra di confronto e l'incasso.

### Modificato
- **Grafica iOS:** titoli grandi che si rimpiccioliscono scorrendo, liste raggruppate, barre traslucide, carattere di sistema.
- La scheda di inserimento ha *Annulla* e *Salva* in alto e si chiude anche trascinandola verso il basso.
- Il menu con le tre lineette non c'è più: Backup, Excel ed eliminazione dei dati sono in *Impostazioni*.

## Versione 3.0 — 16 novembre 2026

Prima versione con **accesso Google** e **dati salvati online**. Parte dalla versione 2.3 di [Granchio-Blu-App-Tracker](https://github.com/TheRealJayser/Granchio-Blu-App-Tracker), che resta com'è.

### Aggiunto
- **Accedi con Google:** all'apertura si sceglie il proprio account Google. Ognuno vede e modifica solo il proprio pescato.
- **Dati nel cloud (Firebase):** ogni uscita viene salvata nell'account. Se il telefono si rompe o si cambia telefono, basta accedere di nuovo per ritrovare tutto.
- **Funziona senza campo:** le modifiche restano in coda sul telefono e partono da sole quando torna la rete. In fondo alla pagina si vede se ci sono modifiche in attesa.
- **Account** in *menu → Impostazioni*: mostra con quale account sei dentro e permette di uscire. Se ci sono dati non ancora inviati, chiede un secondo tocco prima di uscire.

### Modificato
- **Nuovo indirizzo:** l'app è pubblicata su Firebase Hosting, all'indirizzo https://granchio-blu.web.app, al posto di Netlify. Ogni modifica su GitHub va online da sola.
- Import da Excel, ripristino da backup e cancellazione di più giorni vengono inviati in blocco, così sono veloci anche con tanti dati.
- Le librerie Firebase vengono salvate sul telefono, così l'app si apre anche senza connessione.
