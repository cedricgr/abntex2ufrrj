# abntex2ufrrj
Customizações do `abnTeX2` para a Universidade UFRRJ

## Versão 1.0.0 (12 de outubro de 2019)
* Primeira versão publicada

## Como usar
1. Baixe os arquivos `abntex2ufrrj.sty`, `modelo-trabalho-academico.tex` e `logomarca.jpg`.
1. Renomeie o arquivo `modelo-trabalho-academico.tex` para o nome de seu agrado (ex.: `tese.tex`).
1. Siga as instruções no arquivo .tex para alterar os dados necessários (Título, autores, orientadores, instituto, programa de pós-graduação, etc).
1. *Escreva* seu documento usando o modelo renomeado para inserir texto, figuras, etc.
1. Para documentos grandes, uma prática *recomendada* é usar vários arquivos e o comando `input{}` ou `include{}` para inserir trechos do documento (Introdução, Objetivos, ...). Consulte algum manual de uso do LaTeX para detalhes.
1. **Aviso:** a linha que imprime a bibliografia está comentada no documento. Crie seu arquivo BibTeX, edite a linha necessária e remova o comentário para que as referências bibliográficas sejam inseridas corretamente no documento.

## Pré-requisitos
* Uma distribuição TeX instalada e configurada (para Windows recomenda-se [MikTeX](http://miktex.org))
* A classe `abntex2` instalada (MiKTeX instala automaticamente os pacotes que não estiverem instalados se tudo estiver corretamente configurado, *ou se você não tiver desativado esta configuração*)
* A classe `memoir` instalada (abnTeX2 é baseada nela)
* O pacote `times` instalado (o Manual de Teses *exige* Times como fonte no documento)
