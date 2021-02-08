---
title: 'Postazione di Sviluppo'
date: 2021-02-05 21:21:13
category: 'development'
draft: false
---

Di solito quando prendo un nuovo pc la prima cosa che faccio è installare l'editor di sviluppo che, per mia scelta, deve essere anche l'editor di default dei file di testo.
Sono partito tanti anni fa con Sublimetext con cui ho passato veramente tante avventure per poi passare definitivamente a Visual Studio Code il vero gioellino di casa Microsoft con brevi intermezzi di Atom, Vim e Notepad++.

Qualche articolo futuro lo impiegherò per le estensioni che utilizzo di più e le impostazioni delle scorciatoie, per oggi mi limiterò al tema grafico e alcune impostazioni che potrebbero essere utili per tutti.

Apriamo con: ctrl+, il pannello dei settaggi e nelle preferenze utente io metto questo:

````json{codeTitle: "settings.json"}
{
    "workbench.settings.editor": "json",
    "workbench.settings.useSplitJSON": true,
    "workbench.startupEditor": "newUntitledFile",
    "editor.multiCursorModifier": "ctrlCmd",
    "editor.snippetSuggestions": "top",
    "editor.formatOnPaste": true,
    "editor.cursorBlinking": "solid",
    "editor.cursorWidth": 5,
    "explorer.confirmDragAndDrop": false,
    "editor.rename.enablePreview": false,
    "editor.renderWhitespace": "all",
}
````

Non sono molti e soprattutto rendono la vita molto più facile, almeno per me e ora ve li vado a spiegare.

## Workbench

````"workbench.settings.editor": "json"````

Questa impostazione serve per aprire il pannello delle impostazioni utente in formato json invece che in formato grafico (naturalmente come ho detto è questione di preferenze)

````"workbench.settings.useSplitJSON": true````

Questa serve per dividere la visuale delle impostazioni json in due, da una parte i settaggi di Default mentre dall'altra quelli utente, comodo perchè così si ha sempre sotto controllo le proprie impostazioni in relazione a quelle di default

````"workbench.startupEditor": "newUntitledFile"````

Questa impostazione va a modificare la modalità di apertura di Code ovvero invece di mostrare la Welcome Page mostra la finestra di un nuovo file, utile soprattutto quando si usa Code come editor di testo generico

## Editor

````"editor.multiCursorModifier": "ctrlCmd"````

Impostazione che permette di selezionare più stringhe contemporaneamente premendo la combinazione ctrl+cmd che nel caso di Windows e Linux sarà il tasto Alt

````"editor.snippetSuggestions": "top"````

Questo è uno dei grossi limiti di Visual Studio, di default gli snippets di codice vengono mostrati come ultimi risultati costringendo ogni volta a scrivere quasi tutto il comando prima di eliminare le diverse funzioni che non servono oppure muoversi con le freccette per selezionarli, in questo modo invece gli snippets saranon i primi risultati velocizzando per esempio l'inserimento di console.log() in javascript scrivendo log e dando tab.

````"editor.formatOnPaste": true````

Altro elemento fastidiosissimo è la mancata formattazione quando si incolla un testo in un testo già formattato, ogni volta bisogna ripassare le diverse stringhe modificando la formattazione per adattarsi al testo preesistente.

````"editor.cursorBlinking": "solid"````

Questo settaggio va a modificare l'aspetto del cursore che di default blinka ma in maniera poco visibile quindi in questo modo il cursore rimane fisso e con l'opzione successiva andremo a dare uno spessore notevole per renderlo sempre visibile

````"editor.cursorWidth": 5````

Come detto sopra questo fa si che in ogni istante il cursore sia visibile grazie ad uno spessore rilevante

````"editor.rename.enablePreview": false````

Questa opzione farà in modo che facendo click su di un file lo stesso non venga aperto in preview sostituendo il file che abbiamo aperto in visualizzazione ma si aprirà in un nuovo tab non costringendoci ogni volta a splittare la finestra in due per vedere in visualizzazione due file contemporaneamente

````"editor.renderWhitespace": "all"````

Altra impostazione fastidiosa di default è la mancanza di evidenziazione degli spazi, in questo modo a colpo d'occio sapremo sempre quanti spazi sono presenti per ogni riga

## Explorer

````"explorer.confirmDragAndDrop": false````

Ultima impostazione di visualizzazione è la disabilitazione della richiesta di spostare un file ogni volta che lo si trascina, in questo modo non dovremo fare mille click quando andremo a spostare i nostri file.
Spero che queste impostazioni siano utili anche a voi e soprattutto se ne avete di vostre che volete condividere sono curioso di saperle leggendole nei commenti.

Alla prossima

*Alex*
