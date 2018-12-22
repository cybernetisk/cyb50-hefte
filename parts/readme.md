## Tekster

1. Alle kapitler har sin egen .tex-fil, og ligger i sin tilhørende part, e.g. `history/cyb42.tex` (om du ønsker å legge til en ny tekst, snakk med Arne)
2. Skriv artikkelen i ren tekst, uten *documentclass* og lignende LaTeX-markup. Se neste seksjon for tips til LaTeX markup av teksten.
3. Evt. bilder legges i mappen images/, les readme for denne.


### LaTeX-markup av artikler

Artiklene skal **ikke** inneholde kommandoer for `documentclass` eller `usepackage`. Er det behov for spesielle pakker, kontakt Veronika Heimsbakk (veronika.heim@gmail.com).

#### Tekst

Kommandoer for manipulering av font er tillatt.

- fet font: `\textbf{...}`
- kursiv font: `\textit{...}`

**IKKE** bruk kommandoer for større eller mindre tekst (som `\Large{...}` osv.

#### Bilder

Bruk denne formen når du skal legge inn bilder.

```
\begin{figure}
	\includegraphics[width=\textwidth]{img/bildenavn.png}
	\label{fig:bildenavn}
	\caption{Bildebeskrivelse}
\end{figure}
```

Alle bilder *bør* refereres til fra teksten.

#### Eksterne URLer

Om det er behov for eksterne URLer, så kan formen under brukes.

`\href{http://example.org}{Lenkenavn}`

Men husk at tekstene skal publiseres i bokform, så lange, uleselige URLer frarådes.
