README

LaTeX Preamble

Created by Mark Eli Kalderon on 2008-07-30

# Introduction

LaTeX preamble and associated files. Meant to be used as a submodule of a Git repository. The file, preamble.tex, needs to be included in the LaTeX document under version control. See the provided template. For more information about keeping your LaTeX preamble in a Git submodule see this blog [post](http://markelikalderon.com/blog/2008/07/31/keeping-your-latex-preamble-in-a-git-submodule/).

# LaTeX Template

    %!TEX TS-program = xelatex 
    %!TEX TS-options = -synctex=1 -output-driver="xdvipdfmx -q -E"
    %!TEX encoding = UTF-8 Unicode
    %
    %  my_title
    %
    %  Created by my_name on date.
    %  Copyright (c) year. All rights reserved.
    %
    
    \documentclass[12pt]{article} 
    
    % Definitions
    \newcommand\mykeywords{} 
    \newcommand\myauthor{} 
    \newcommand\mytitle{}
    \newcommand\mybib{}
    
    \include{preamble/preamble.tex}
    
    %%% BEGIN DOCUMENT
    \begin{document}

    % Title Page
    \maketitle
    % \begin{abstract} % optional
    % \noindent
    % \end{abstract} 
    \vskip 2em \hrule height 0.4pt \vskip 2em
    % \epigraph{text of epigraph}{\textsc{author of epigraph}} % optional; make sure to uncomment \usepackage{epigraph}
    
    % Layout Settings
    \setlength{\parindent}{1em}

    % Main Content
    
    
    
    % Bibligography
    \bibliographystyle{plainnat} 
    \bibliography{\mybib} 
    
    \end{document}

# License

The files:

* preamble.tex
* README.markdown

are written by Mark Eli Kalderon <mailto:eli@markelikalderon.com> and are dedicated to the Public Domain.
