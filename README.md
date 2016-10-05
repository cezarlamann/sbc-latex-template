# sbc-latex-template
Template LaTeX para a SBC - Sociedade Brasileira de Computação (LaTeX template for SBC - Brazilian Computation Society)

## Observações - Disclaimer
#### (PT-BR) Eu não sou o autor original deste template. Recebi de um orientador de graduação e apenas estou postando aqui para facilitar o desenvolvimento de trabalhos futuros. Desconheço os autores originais. Caso alguém conheça, por favor submeta um pull-request para realizar os devidos créditos e/ou correções.
#### (EN) I'm not the original author of this template. I received this template from a former graduation teacher and I'm only posting here to ease future works development. I don't even know who is or whose are the author(s). Just in case someone knows, please submit a pull-request to do the proper credits and/or related bugfixes.

## Para quem está começando:

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
