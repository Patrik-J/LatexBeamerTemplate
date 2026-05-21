# Latex Beamer Template

This git serves to store my personal LaTeX template for beamer presentations.

## Usage

After cloning the git or downloading the files, ensure that your main .tex file is in the same folder as the git contents.

Before starting, you need to either comment out the part responsible for the include pngs, or define *logo.png* and *titleLogo.png* in the same folder as the package.

First off, in your main .tex file you need to use the beamer document class and include this package. After, you can work on your presentation. :D

Here a minimal working example.
```latex

    \documentclass{beamer}
    
    \usepackage{beamerPackage}

    ... 

    \InitBeamer{Big Title}[Short Title]{Subtitle}{Author}[Short Author]{Insitute}[Short Institute][\today]

    % if the navigation bar should not be shown
    \beamertemplatenavigationsymbolsempty

    \NoHeader{}
    \InBetweenTOC{}
    \InBetweenSubTOC{}

    \begin{document}
        \showtitle{}

        \begin{frame}
            \frametitle{Table of Contents}
            \tableofcontents
        \end{frame}

    \end{document}
```