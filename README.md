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
