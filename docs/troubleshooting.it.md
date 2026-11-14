# Risoluzione dei problemi — Head Tracker+Voice+Instructor

🌐 [English](troubleshooting.en.md) · [Русский](troubleshooting.ru.md) · [Français](troubleshooting.fr.md) · [Deutsch](troubleshooting.de.md) · Italiano

Trova il tuo sintomo e segui i passi nell’ordine. Se niente funziona, [invia un rapporto](#inviare-un-rapporto-allo-sviluppatore).

## Installazione

### «PC protetto da Windows» — non si riesce ad andare avanti
Fai clic su **Ulteriori informazioni**, poi su **Esegui comunque**. Se il pulsante **Esegui comunque** non c’è, è attivo il Controllo intelligente delle app: vedi [Installazione, passo 2.5](install.it.md).

### Il browser non vuole tenere il file scaricato
Edge: **…** → **Mantieni** → **Mostra altro** → **Mantieni comunque**. Chrome: fai clic sul file → **Scarica file non sicuro**.

### Il primo avvio è molto lento
Microsoft Defender sta controllando il nuovo programma; può richiedere fino a un minuto. Aspetta.

### L’installazione dice che il programma è in esecuzione e va chiuso
Chiudi il programma con **File → Esci** (non basta la ✕ della finestra), poi avvia di nuovo l’installazione.

## Collegamento dell’iPhone

### L’app sull’iPhone dice che non c’è collegamento con il PC
1. Il programma sul PC deve essere avviato.
2. **Cavo:** collegalo, sblocca l’iPhone e rispondi **Autorizza** se chiede «Autorizzare questo computer?».
3. **Wi-Fi:** il PC e l’iPhone devono essere sulla stessa rete.
4. Tocca **Riprova** nell’app.

### Il collegamento funzionava, poi si è interrotto durante il volo
1. Controlla il cavo (o il Wi-Fi).
2. Fai di nuovo clic su **Avvia** nel programma sul PC.
3. Se l’app indica una qualità Wi-Fi scarsa, usa il cavo o avvicinati al router.

### L’iPhone sembra a posto, ma il PC dice «volto non visibile»
1. Nel programma sul PC apri **Impostazioni → iPhone** e scegli di nuovo il collegamento (cavo o Wi-Fi).
2. Fai di nuovo clic su **Avvia**.

### Con il cavo, a volte l’iPhone non viene trovato
1. Scollega e ricollega il cavo, con l’iPhone sbloccato.
2. Chiudi gli altri programmi che usano l’iPhone come fotocamera o webcam.
3. Prova un altro cavo o un’altra porta del PC.

## Tracciamento della testa

### La visuale non si muove
1. In basso nella finestra principale: c’è la scritta verde **IN FUNZIONE**? Se no, fai clic su **Avvia**.
2. Nel riquadro Visuale: c’è scritto **volto visibile**? Se no, vedi sotto.
3. Siediti dritto e fai clic su **Centra** (Ctrl+Alt+C).
4. Controlla che la **Pausa** non sia attiva (Ctrl+Alt+X la attiva e la disattiva).

### «Volto non visibile»
- L’iPhone deve essere rivolto verso di te, a circa un braccio di distanza, senza nulla tra te e la fotocamera.
- Evita una luce forte proprio dietro la testa.
- Se ti sei coperto il viso per un attimo, il tracciamento riprende da solo dopo qualche secondo.

### La visuale è lenta, a scatti o troppo sensibile
**Profili → Impostazioni della visuale** → fai clic sulla curva pronta **Caccia** o **Civile**. Poi regola con precisione **Sensibilità** e **Smorzamento** nella finestra principale.

### La visuale va nella direzione sbagliata (a sinistra invece che a destra)
Apri **Profili → Impostazioni della visuale**. Nell’elenco **Assi** fai clic sull’icona ⇄ a destra di quell’asse (⇄ = invertito). Poi, per favore, [segnalalo](https://github.com/liaison-studio/htvi/issues/new/choose) indicando il nome del simulatore: la direzione dovrebbe essere giusta senza modifiche.

### Col tempo la visuale si sposta dal centro
Siediti dritto e premi **Ctrl+Alt+C** (oppure di’ «centra la vista»). Per correggerla in automatico, attiva **Ricentraggio lento** in **Profili → Impostazioni della visuale**.

## Comandi vocali

### Un comando non viene riconosciuto
1. La lingua dei comandi nel programma per PC (**Impostazioni → Voce**) e la lingua del parlato sull’iPhone (**Impostazioni → Lingua del parlato**) devono essere uguali. Se sono diverse, la finestra principale mostra un avviso giallo.
2. Se usi il PTT, tieni premuto il pulsante mentre parli.
3. Parla in modo breve, come un pilota: «carrello giù», non una frase lunga.
4. L’elenco delle frasi per il tuo gioco è nella finestra **Comandi**.

### Un comando è stato riconosciuto, ma nel gioco non è successo niente
Fai clic su **Non funziona: disattiva** sotto l’ultimo comando. Il programma lo annota, così il comando può essere corretto. Per favore, [segnalalo](https://github.com/liaison-studio/htvi/issues/new/choose) anche a noi, con la frase e il simulatore.

## Istruttore

### L’istruttore non parla
Windows non ha una voce per la tua lingua. **Impostazioni di Windows → Ora e lingua → Voce → Aggiungi voci**, aggiungi una voce per la tua lingua, poi riavvia il programma.

### L’istruttore segue l’aereo sbagliato
Nel riquadro Istruttore scegli tu l’aereo invece di **Auto**.

## Inviare un rapporto allo sviluppatore
1. **Assistenza → Rapporto per lo sviluppatore…**
2. Descrivi cosa è successo.
3. Fai clic su **Salva l'archivio…**. L’archivio viene salvato in *Documenti → Head Tracker Voice Instructor → Reports*.
4. Allegalo a una [segnalazione di bug](https://github.com/liaison-studio/htvi/issues/new/choose) oppure invialo a liaison.studio.contact@gmail.com.

Il rapporto non contiene audio né dati di associazione. Il programma non invia mai nulla di sua iniziativa.
