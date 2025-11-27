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
- [](#)
- [Comandos Úteis](#comandos-úteis)
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
" Primeiro documento ---------------- {{{
-->
## Primeiro documento

Ao criar um documento no LaTeX, devem ser declarados alguns parâmetros do seu início, ou _preâmbulo_, como é chamado. Todos esses parâmetros são precedidos por uma _contrabarra_ '\'. 

O primeiro deles é o tipo ou classe de documento:  

\documentclass{article} (Classes listadas em @TODO)

Para iniciar o documento em si, usa-se o parâmetro '_begin_':

\begin{document}

Este parâmetro deve ser seguido de '_\end{document}_' ao final. 


<sub>[⬆](#sumário)</sub>
---
<!--
" }}}
-->
