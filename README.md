# Notes

Questa è la repository in cui carico il codice $\LaTeX$ dei miei appunti. Se dovessero esserci errori, non esitare a scrivermi! 😉

## Indice

- [Perché Github](#why-github)
- [Visualizzare il pdf](#viewing-pdf)
- [Aggiornare il pdf](#updating-pdf)
- [Flashcards](#flashcards)

<a id="why-github"></a>

## Perché Github

Ho deciso di utilizzare Github e Git perché così non devo seguire una procedura lunghissima (scaricare il pdf, andare su Google Drive, eliminare quello caricato precedentemente e caricare quello nuovo), ma semplicemente con tre comandi da terminale aggiorno tutto (per i curiosi: `git add .`, `git commit -m "<messaggio>"` e `git push`).

Uso poi Github anche per fare un backup del codice: non si sa mai che, per qualche strano motivo, Overleaf non dovesse funzionare in futuro 🤷‍♂️

L'unico problema di utilizzare Github senza caricare anche i pdf, è che di volta in volta devi generartelo tu (nulla di complicato). Pensala magari così: anziché avere sempre gli appunti pronti qui, devi impegnarti a creare i tuoi e, solo nel caso tu non capisca qualcosa, allora segui la procedura qui sotto. Ovviamente, essendo uno studente anch'io, non garantisco che le spiegazioni nei miei appunti siano sempre chiare!

<a id="viewing-pdf"></a>

## Visualizzare il pdf

Per non aver problemi in futuro con il limite della grandezza dei file caricabili su Github, ho deciso di caricare solamente codice ed immagini.

Dato il codice e le immagine ci sono diversi modi per generare il file pdf. Io ti guiderò in quello più semplice:

1. Vai su [Overleaf](https://www.overleaf.com/project) e crea un account (oppure, se già lo hai, accedi).

2. Utilizza il tasto verde "New Project" (o "Nuovo Progetto" a seconda della lingua) in alto a sinistra nella sidebar, seleziona la voce "Blank Project" (o "Progetto Vuoto") e scegli il nome che preferisci (sarà il nome del tuo file pdf). Tranquillo puoi anche cambiarlo in seguito.

3. Ora dovresti avere l'editor Overleaf aperto, con tre parti: la sidebar in cui navigare tra i tuoi file, l'editor in cui scrivere codice $\LaTeX$ e la preview del pdf. Cancella tutto quello che c'è scritto nell'editor. Indicativamente, dovrebbe esserci scritto una roba del genere:

```latex
\documentclass{article}
\usepackage{graphicx} % Required for inserting images

\title{Nome del progetto}
\author{Nome del tuo account}
\date{Mese Anno}

\begin{document}

\maketitle

\section{Introduction}

\end{document}
```

4. Ora spostati su Github e apri il file `main.tex`. Utilizza quindi il tasto in alto a destra per copiarne il contenuto (se non lo trovi, seleziona tutto il codice e copialo).

5. Ritorna su Overleaf e incolla ciò che hai copiato sull'editor. Ora se hai seguito tutti i passaggi correttamente, cliccando il tasto verde "Recompile" in alto, dovrebbe uscirti il pdf. Ora mancano solo le immagini!

6. Ritorna quindi su Github e scarica tutte le immagini dentro l'apposita cartella (purtroppo il processo è un po' lungo: devi cliccare sopra ogni singola immagine e poi compare il tasto per scaricarle, sempre in alto a destra).

7. Una volta scaricate tutte le immagini, all'interno dello stesso progetto di Overleaf di prima, crea una cartella chiamata "images" (chiamala **esattamente** uguale dato che i path delle immagini contengono quella). Per farlo ti basta cliccare il tasto a forma di cartella nella sidebar, appena sotto la scritta "Menu".

8. Infine, trascina le immagini sopra il nome della cartella e clicca il tasto "Upload".

Ricapitolando, quindi, la struttura finale del tuo progetto dovrebbe essere la seguente:

```tree
|--images
   |--imageOne
   |--imageTwo
   |--...
|--main.tex
```

Se hai fatto tutto correttamente, dopo aver cliccato nuovamente il tasto "Recompile", dovresti riuscire a visualizzare il mio stesso pdf. Non ti basta ora che scaricarlo (c'è il tasto vicino alla scritta "Recompile") e studiarlo 🥲

<a id="updating-pdf"></a>

## Aggiornare il file pdf

Cercherò di aggiornare periodicamente il file e quindi di caricare qui nuove versioni del codice.

Se hai già seguito la procedura qui sopra e vuoi semplicemente aggiornare il file:

1. Apri il progetto su [Overleaf](https://www.overleaf.com/project).

2. Visualizza il codice $\LaTeX$ su Github e copialo sempre utilizzando il tasto in alto a destra.

3. Seleziona tutto il codice $\LaTeX$ presente sull'editor Overleaf con il comando:

```
  Windows/Linux: Ctrl+A
  MacOS: Cmd+A
```

4. Incolla il nuovo codice con:

```
  Windows/Linux: Ctrl+V
  MacOS: Cmd+V
```

5. Controlla che non siano state inserite nuove immagini sulla cartella `images` di Github. In caso, segui la procedura dal punto 6. al punto 8. di [Visualizzare il pdf](#viewing-pdf).

<a id="flashcards"></a>

## Flashcards

All'interno di questa repository trovi anche un altro file chiamato `Flashcards.md`, in cui scrivo delle domande ipotetiche da esame (ovviamente non so se sono da esame, perché non ho mai fatto un esame universitario in vita mia, ma perlomeno sono domande di teoria che cercano di trattare tutti gli argomenti affrontati 😅).

Per renderizzare il file markdown aprilo su Github oppure utilizza un qualcosa del tipo [Markdown Live Preview](https://markdownlivepreview.com/).

Come per il codice e le immagini, cercherò di aggiornare progressivamente anche questo file.
