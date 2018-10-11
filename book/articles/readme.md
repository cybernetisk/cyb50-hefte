## Artikler

1. Opprett fil med *kapittelnr-artikkelnavn*.tex (kapittelnr finner du i table of contents i book.pdf)
2. Skriv artikkelen i ren tekst, uten *documentclass* og lignende LaTeX-markup. Se neste seksjon for tips til LaTeX markup av teksten.
3. Evt. bilder legges i mappen img/, les readme for denne.


### LaTeX-markup av artikler
Artiklene skal **ikke** inneholde kommandoer for `documentclass` eller `usepackage`. Er det behov for spesielle pakker, kontakt Veronika Heimsbakk (veronika.heim@gmail.com).
#### Tekst
Kommandoer for manipulering av font er tillatt.
- fet font: `\textbf{...}`
- kursiv font: `\textit{...}`

**IKKE** bruk kommandoer for større eller mindre tekst (som `\Large{...}` osv.

#### Bilder
```
\begin{figure}
	\includegraphics[width=\textwidth]{img/bildenavn.png}
	\label{fig:bildenavn}
	\caption{Bildebeskrivelse}
\end{figure}
```

Alle bilder *bør* refereres til fra teksten.

#### Eksterne URLer
`\href{http://example.org}{Lenkenavn}`
