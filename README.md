# abntex2ufrrj
Customizações do `abnTeX2` para a Universidade UFRRJ 

## Versão atual: 1.1.0 (14 de outubro de 2019)
* Segunda versão publicada (consulte o [CHANGELOG](CHANGELOG.md) para detalhes)

## O que há no `abntex2ufrrj`?
* O `abntex2ufrrj` existe por um motivo: *embora o Manual de Teses da UFRRJ diga que siga as normas da ABNT, ele não segue*
* Além dos ambientes personalizados do abnTeX2, há a inclusão dos ambientes `quadro` e `esquema` (sendo que o ambiente quadro já existia personalizado no modelo canônico que vem junto com o abnTeX2), e os comandos `\listofquadros` e `\listofesquemas` para imprimir, respectivamente, a *Lista de Quadros* e de *Esquemas*. **NOTA:** a inclusão de Esquemas não existe no Manual de Teses da UFRRJ, mas ela é muito utilizada em Teses e Dissertações na área Química e, portanto, foi incluida aqui.
* Os comandos `\imprimircapa` e `\imprimirfolhaderosto` foram alterados para adequar a Capa e Folha de Rosto ao Manual
* Foram incluídos os comandos `\instituto{}` e `\programapg{}`, assim como suas contrapartes `\imprimirinstituto` e `\imprimirprogramapg` para se preencher o nome do Insituto e Programa de Pós-Graduação de maneira separada da `\instituicao{}`
* Os tamanhos de fontes dos títulos de capítulos e seções foram alterados
* A numeração de página foi alterada para que a página 1 seja a primeira página da Introdução (*de acordo com o Manual, não há a necessidade de se numerar a parte pré-textual*)

## O que virá em versões futuras
* Opcionalmente, a possibilidade de numeração em algarismos romanos na parte pré-textual
* Modelos adicionais para a Tese/Dissertação em *Capítulos* e como *Narrativa em Capítulos*, incluindo gerenciamento de múltiplas referências bibliográficas no documento.

## Como usar
1. Baixe os arquivos `abntex2ufrrj.sty`, `modelo-trabalho-academico.tex` e `logomarca.jpg`.
1. Renomeie o arquivo `modelo-trabalho-academico.tex` para o nome de seu agrado (ex.: `tese.tex`).
1. O pacote tem duas opções: `[versao=banca]` (padrão caso o pacote não tenha opções declaradas) ou `[versao=final]`, que alteram o espaçamento entre linhas de 1,5 para 1, respectivamente. 
1. Siga as instruções no arquivo .tex para alterar os dados necessários (Título, autores, orientadores, instituto, programa de pós-graduação, etc). Recomenda-se também alterar a seção PDFBOOKMARKS.
1. *Escreva* seu documento usando o modelo renomeado para inserir texto, figuras, etc.
1. Para documentos grandes, uma prática *recomendada* é usar vários arquivos e o comando `input{}` ou `include{}` para inserir trechos do documento (Introdução, Objetivos, ...). Consulte algum manual de uso do LaTeX para detalhes.
1. **Aviso:** a linha que imprime a bibliografia está comentada no documento. Crie seu arquivo BibTeX, edite a linha necessária e remova o comentário para que as referências bibliográficas sejam inseridas corretamente no documento.

## Pré-requisitos
* Uma distribuição TeX instalada e configurada (para Windows recomenda-se [MikTeX](http://miktex.org))
* A classe `abntex2` instalada (MiKTeX instala automaticamente os pacotes que não estiverem instalados se tudo estiver corretamente configurado, *ou se você não tiver desativado esta configuração*)
* A classe `memoir` instalada (abnTeX2 é baseada nela)
* O pacote `times` instalado (o Manual de Teses *exige* Times como fonte no documento)
