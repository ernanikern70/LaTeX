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
\documentclass[a4paper,10pt]{article}

\usepackage[utf8]{inputenc} % pacote para acentuação
\usepackage[brazil]{babel} % coloca os nomes em pt-br
\usepackage{indentfirst} % aplica indentação
%\usepackage{fontenc}

\date{27/11/2025}

% CORPO DO TEXTO
\begin{document}
\section{Seção antes da seção 1}
No mundo atual, a competitividade nas transações comerciais ressalta a relevância da participação ativa da articulação interinstitucional necessária. Considerando as lições aprendidas, a valorização de fatores subjetivos não pode mais se dissociar de alternativas às soluções ortodoxas. Não obstante, a expansão dos mercados mundiais apresenta tendências no sentido de aprovar a manutenção das condições inegavelmente apropriadas. O empenho em analisar a necessidade de renovação processual legitima a busca por soluções sistêmicas dos níveis de motivação departamental.    \section{Seção 1}
É importante questionar o quanto a adoção de políticas descentralizadoras ainda não demonstrou convincentemente que vai participar na mudança das rupturas provocadas pela transformação digital. As experiências acumuladas demonstram que o desenvolvimento contínuo de distintas formas de atuação modifica os parâmetros tradicionais de análise dos conhecimentos estratégicos para atingir a excelência.

Evidentemente, a complexidade dos estudos efetuados deve passar por modificações independentemente do fluxo de informações. À luz das boas práticas institucionais, a consulta aos diversos militantes é uma das consequências dos instrumentos regulatórios vigentes.
% para abrir parágrafo, deixar linha anterior em branco
\subsection{Subseção x.x}
Vale destacar que o início da atividade geral de formação de atitudes exige a precisão e a definição das novas proposições. Por intermédio de análises qualificadas, a valorização da diversidade de pensamento talvez venha a ressaltar a relatividade das condições estruturais subjacentes.\\ De acordo com especialistas, a crescente influência da mídia faz parte de um processo de gerenciamento das regras de conduta normativas.\\ Ainda assim, existem dúvidas a respeito de como a revolução dos costumes agrega valor ao estabelecimento dos aprendizados oriundos da experiência acumulada.
% o '\\' gera quebra de linha
\subsubsection*{Subseção x.x.x}
A prática cotidiana prova que o aumento do diálogo entre os diferentes setores produtivos nos obriga à análise do remanejamento dos quadros funcionais. Pensando mais a longo prazo, a hegemonia do ambiente político oferece uma interessante oportunidade para verificação do processo de comunicação como um todo. Percebemos, cada vez mais, que a redefinição dos modelos de governança aprofunda o debate sobre a sustentabilidade dos processos que moldam a realidade institucional.
% o '*' na '\subsubsection' elimina a numeração da seção; se houver nova seção após, a numeração continuará a partir da última numerada.

\subsubsection{Subseção x.x.x}
Podemos já vislumbrar o modo pelo qual a expansão dos canais de diálogo social auxilia a preparação e a composição das formas de ação. Assim mesmo, a estruturação de redes de cooperação intersetorial aponta para a melhoria da governabilidade em ambientes voláteis. Neste sentido, o julgamento imparcial das eventualidades maximiza as possibilidades por conta da gestão inovadora da qual fazemos parte. O que temos que ter sempre em mente é que a constante divulgação das informações representa uma abertura para a melhoria da inteligência coletiva mobilizada. Caros amigos, o acompanhamento das preferências de consumo causa impacto indireto na reavaliação dos índices pretendidos.

\end{document}

```
PS: o '*' na '\subsubsection' elimina a numeração da seção; se houver nova seção após, a numeração continuará a partir da última numerada.

Ao inserir seções numeradas anteriores à outras existentes, o LaTeX fará os ajustes. 

<sub>[⬆](#sumário)</sub>
---
<!--
" }}}
-->
