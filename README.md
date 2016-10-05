# sbc-latex-template
Template LaTeX para a SBC - Sociedade Brasileira de Computação (LaTeX template for SBC - Brazilian Computation Society)

### Autor/Fonte original (Original Author): SBC - Sociedade Brasileira de Computação

http://www.sbc.org.br/documentos-da-sbc/summary/169-templates-para-artigos-e-capitulos-de-livros/878-modelosparapublicaodeartigos

## Para quem está começando:

### LaTeX em 157 minutos:

 - http://tug.ctan.org/info/lshort/english/lshort.pdf

### Windows:
#### Antes de continuar:
 Eu recomendo, particularmente falando, que a instalação do MiKTeX e do TeXstudio seja feita por meio da ferramenta Chocolatey (https://chocolatey.org/) pois ela já seta variáveis de ambiente e mais algumas coisas para facilitar o seu trabalho.
 - Instale o programa MiKTeX, disponível em http://miktex.org/download
 - Abra o gerenciador de pacotes (como administrador).
 - Verifique se você tem instalado os seguintes pacotes: graphicx, url, babel, enumitem e placeins. Caso não tenha, realize a instalação dos mesmos, marcando para instalação (Botão "+" na barra superior).
 - Como editor padrão para o LaTeX, indico o TeXstudio (http://www.texstudio.org/ - na instalação ele já configura os caminhos padrão das ferramentas do MiKTeX), porém fica à critério.

#### Instalação via Chocolatey
 - Em um prompt de comando (Administrador) (`cmd.exe`), digite: `choco install miktex texstudio -y` 
 - Pronto! Et voilà!

### Como usar o template:
 - Clone o repositório, ou baixe-o no formato `.zip`.
 - Abra o arquivo `.tex` no seu editor favorito
 - Mande o seu editor fazer a compilação ou então faça manualmente usando os comandos:
  - `latex.exe -src -interaction=nonstopmode <MEU_ARQUIVO_TEX>.tex` 
  - `pdflatex.exe -synctex=1 -interaction=nonstopmode <MEU_ARQUIVO_TEX>.tex` 

### Como formatar códigos-fonte dentro dos templates LaTeX:

    %Adicionar os pacotes abaixo no topo do seu documento
	
	\usepackage{listings}
    \usepackage{color}
    
	%Definir cores para realce de código (OPCIONAL, mas se for feito, fazer logo abaixo das tags "\usepackage")
    \definecolor{mygreen}{rgb}{0,0.6,0}
    \definecolor{mygray}{rgb}{0.5,0.5,0.5}
    \definecolor{mymauve}{rgb}{0.58,0,0.82}
    
	%Definir configurações gerais
	
    \lstset{ %
	    language=Python,                 % LINGUAGEM DO CÓDIGO. DEFINIR AQUI SE FOR UTILIZAR SOMENTE UMA LINGUAGEM.
        backgroundcolor=\color{white},   % choose the background color; you must add \usepackage{color} or \usepackage{xcolor}
        basicstyle=\footnotesize,        % the size of the fonts that are used for the code
        breakatwhitespace=false,         % sets if automatic breaks should only happen at whitespace
        breaklines=true,                 % sets automatic line breaking
        captionpos=b,                    % sets the caption-position to bottom
        commentstyle=\color{mygreen},    % comment style
        deletekeywords={...},            % if you want to delete keywords from the given language
        escapeinside={\%*}{*)},          % if you want to add LaTeX within your code
        extendedchars=true,              % lets you use non-ASCII characters; for 8-bits encodings only, does not work with UTF-8
        frame=single,	                   % adds a frame around the code
        keepspaces=true,                 % keeps spaces in text, useful for keeping indentation of code (possibly needs columns=flexible)
        keywordstyle=\color{blue},       % keyword style
        otherkeywords={*,...},           % if you want to add more keywords to the set
        numbers=left,                    % where to put the line-numbers; possible values are (none, left, right)
        numbersep=5pt,                   % how far the line-numbers are from the code
        numberstyle=\tiny\color{mygray}, % the style that is used for the line-numbers
        rulecolor=\color{black},         % if not set, the frame-color may be changed on line-breaks within not-black text (e.g. comments (green here))
        showspaces=false,                % show spaces everywhere adding particular underscores; it overrides 'showstringspaces'
        showstringspaces=false,          % underline spaces within strings only
        showtabs=false,                  % show tabs within strings adding particular underscores
        stepnumber=2,                    % the step between two line-numbers. If it's 1, each line will be numbered
        stringstyle=\color{mymauve},     % string literal style
        tabsize=2,	                   % sets default tabsize to 2 spaces
        title=\lstname                   % show the filename of files included with \lstinputlisting; also try caption instead of title
    }
