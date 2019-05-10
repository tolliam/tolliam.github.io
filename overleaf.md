## Overleaf/LaTeX

### Create new project
`New project >> Upload Project >> Select a .zip file`

### Export
`Menu >> PDF`

### Import figure, .tex, .bib, .pdf  to project

![Import](upload.jpeg "upload")

### In text citation
`\cite{RefWorks:xxxxxx}`

### Cross reference
`~\ref{figure or table label}`

### Tables
`\begin{table}[hbt!]`  
`\footnotesize`  
`\centering`  
`\caption{Table_caption}`  
 `\begin{tabular}{||c|cc|} `  
` \hline`  
 `Column_head1 & Column_head2 & Column_head3 \\ [0.5ex] `  
 `\hline`  
 `Row 1 & 72 & 30  \\ `  
   `\hline`  
 `Row2 & 47 & 0   \\`  
    `\hline`  
`\end{tabular}`  
`\label{table_label}`  
`\end{table}`  

### Figures 

`\begin{figure}[hbt!]`  
`	\centering`  
`\caption{fig_caption}`  
	`\includegraphics[width=0.7\linewidth]{figname.png}`  
`	\label{fig_label}`  
`\end{figure}`  

[Change figure position](https://www.overleaf.com/learn/latex/Positioning_of_Figures)

### Subfigures
`\begin{figure}[h]`  
`\begin{subfigure}{0.5\textwidth}`  
`\includegraphics[width=1.1\linewidth, height=11cm]{Figure/xxxx.png}`  
`\caption{subfigure1_captionhere}`  
`\label{subfig_label1}`  
`\end{subfigure}`  
`\begin{subfigure}{0.5\textwidth}`  
`\includegraphics[width=1.1\linewidth, height=11cm]{Figure/yyyy.png}`  
`\caption{subfigure2_captionhere}`  
`\label{subfig_label2}`  
`\end{subfigure}`  

### Inserting PDF
`\usepackage{pdflscape}`
`\usepackage{pdfpages}`

`\includepdf[pages=-]{pdfname.pdf}`


### Single landscape page

`\usepackage{geometry}`

`\newgeometry{margin=0.3cm}`  
`\begin{landscape}`  
`\thispagestyle{empty}`  

`\end{landscape}`
`\restoregeometry`
