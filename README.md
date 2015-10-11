# Survey package for latex

## Example:

```
\documentclass{scrartcl}

\usepackage{fragebogen}


% documentstart
\begin{document} 

% scrartcl metadata
\title{Survey}
\author{John Doe}
\date{\today}
\maketitle

% questionblock
\begin{questionblock}{Title of the Questionblock}

  % multiple choice question
  \begin{question}{Question}
    \item Answer 1
    \item Answer 2
    ...
  \end{question}
  
  % multiple choice question with a picture
  \begin{picquestion}[Picturewidth]{Question}{Path to Picture}
		\item Answer 1
    \item Answer 2
    ...
  \end{picquestion} 
  
\end{questionblock}

% questionblock
\begin{questionblock}{Title of the Questionblock}

  % question with a free text field
  \textquestion{Question}{Vertical space of the text field}
  
  % question with a free text field and a picture
  \textquestion[Picturewidth]{Question}{Vertical space of the text field}{Path to Picture}
  
\end{questionblock}

\end{document}
```