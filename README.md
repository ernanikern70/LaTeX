<!--
" Badges ------------------ {{{
-->
<!-- Estes badges só funcionarão quando o repositório do github for público -->
![GitHub repo size](https://img.shields.io/github/repo-size/ernanikern70/LaTeX?label=Repo%20size&style=flat-round&logo=github) 
![GitHub branch status](https://img.shields.io/github/checks-status/ernanikern70/LaTeX/main) 
![Last commit](https://img.shields.io/github/last-commit/ernanikern70/LaTeX?label=Last%20commit&style=flat-round&color=green) 
![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/ernanikern70/LaTeX)
![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/ernanikern70/LaTeX)
![GitHub stars](https://img.shields.io/github/stars/ernanikern70/LaTeX?label=%E2%AD%90%20Stars&style=flat-square&color=yellow)
![GitHub followers](https://img.shields.io/github/followers/ernanikern70) 
<!--
" }}}
-->
<!--
" Sumário ----------------------- {{{
-->
### Sumário

- [Instalação](#instalação)
- [Definições](#definições)
- [Primeiro documento](#primeiro-documento)
- [Editores](#editores)

---
<!---
" }}}
-->
<!--
 " Instalação --------------------------- {{{
-->
## Instalação 

### Instalação do LaTeX no Ubuntu

```
sudo apt install texlive-full
```
_Instala o texlive com todas as extensões, mais demorado e ocupa espaço, mas é mais prático._

### Instalação de um editor 

Existem vários editores disponíveis, como o Kile, TeXStudio, e outros, inclusive de que funcionam de forma _online_. 

No momento de criação deste manual estou estudando o [Kile](https://kile.sourceforge.io/), que pode ser instalado via repositórios do Ubuntu. 

<sub>[⬆](#sumário)</sub>
---
<!--
" }}} 
-->
<!--
" Definições -------------------- {{{
-->
## Definições

O LaTeX é um processador de textos com linguagem própria, que não segue o modelo _WYSIWYG - What you see is what you get_. Entretando, há vários editores que permitem pré-visualização dos documentos enquanto são editados.  
Os documentos LaTeX são salvos com a extensão _.tex_, e após terem seus códigos compilados, geram os documentos em _.pdf_.

<sub>[⬆](#sumário)</sub>
---
<!--
" Primeiro documento ---------------- {{{
-->
## Primeiro documento

Ao criar um documento no LaTeX, devem ser declarados alguns parâmetros do seu início, ou _preâmbulo_, como é chamado. Todos esses parâmetros são precedidos por uma _contrabarra_ '\'. 

O primeiro deles é o tipo ou classe de documento:  
```
\documentclass{article} 
```
As diversas classes podem ser encontradas em @TODO.

Para iniciar o documento em si, usa-se o parâmetro '_begin_':
```
\begin{document}
```
Este parâmetro deve ser seguido de ```\end{document}``` ao final. 

Os dois parâmetros acima são obrigatórios, e existem vários opcionais. 

#### Comentários

Como é um código, o LaTeX permite comentários. Para isso, usar '%', no início ou meio da linha. 

Para que o '%' não seja considerado comentário, usar como comando: '\\%'. 

__PS__: Alguns caracteres especiais, como '&', também precisam ser precedidos de '\\'. 

#### Primeiro exemplo de documento

```
% PREÂMBULO
\documentclass[a4paper,10pt]{article} % define a classe do doc e outras opções
\usepackage[brazil]{babel} % este pacote coloca os nomes em pt-br
\usepackage[utf8]{inputenc} % pacote para acentuação
\usepackage{indentfirst} % aplica indentação

%\usepackage{fontenc}

\date{27/11/2025}

% CORPO DO TEXTO
\begin{document}
    \section{Seção 1}

    Meu primeiro documento. Meu primeiro documento. Meu primeiro documento. Meu primeiro documento. Meu primeiro documento. Meu primeiro documento. Meu primeiro documento.

    Segunda linha. % para abrir parágrafo, deixar linha anterior em branco
    \subsection{Subseção 1.1}
    Músicas:
      É isso aí
      Onde estará o meu amor
    \subsubsection*{Subseção 1.1.1} 
    ```
    ```
      Nick Cave \& The Bad Seed

\end{document}
```
PS: o '*' na '\subsubsection' elimina a numeração da seção; se houver nova seção após, a numeração continuará a partir da última numerada.

Ao inserir seções numeradas anteriores à outras existentes, o LaTeX fará os ajustes. 

<sub>[⬆](#sumário)</sub>
---
<!--
" }}}
-->
