---
title       : Introdução ao uso do Linux
subtitle    : Conceitos básicos e instalação
author      : Fernando de Pol Mayer
date        : 2013-09-02
job         : ESALQ/USP
logo        : Tux.svg
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
assets      :
  css: "http://netdna.bootstrapcdn.com/font-awesome/3.2.1/css/font-awesome.css"
---

<br><br><br><br>
### Slides disponíveis em [http://fernandomayer.github.io/linux-intro](http://fernandomayer.github.io/linux-intro)

### Feito com [Slidify](http://slidify.org)

### Código-fonte disponível no [GitHub](https://github.com/fernandomayer/linux-intro/tree/gh-pages)

### Pressione "o" para visualizar miniaturas

### Use <i class="icon-arrow-left"> &nbsp; </i><i class="icon-arrow-right"></i> para navegar

---

## Plano do curso

* Software Livre
* Características do Linux
* Principais distribuições
* Contas de usuários
* Comandos básicos
* `...`

--- .segue .nobackground .dark

## Software Livre

--- &twocol

## Software Livre

Richard Stallman - Projeto GNU (1983)

*** =left

<div class="centered">
<img src="assets/img/RMS.jpeg" width=80%/>
</div>

*** =right

<div class="centered">
<img src="assets/img/GNU.png" width=80%/>
</div>

--- &twocol

## Software Livre

Linus Torvalds - Linux (1991)

*** =left

<div class="centered">
<img src="assets/img/LT.jpeg" width=60%/>
</div>

*** =right

<div class="centered">
<img src="assets/img/Tux.svg" width=60%/>
</div>

--- &twocol

<br><br><br>
<center>
## GNU + Linux = GNU/Linux
</center>
<br><br>
*** =left

<div class="centered">
<img src="assets/img/GNU.png" width=60%/>
</div>

*** =right

<div class="centered">
<img src="assets/img/Tux.svg" width=60%/>
</div>

---

## Software Livre

### O que é software livre?

- Software que pode ser utilizado, estudado e modificado sem
    restrições

- Pode ser copiado e redistribuido (modificado ou não)

- A redistribuição tem uma única restrição: assegurar que os
    receptores tenham a mesma liberdade

- Para isso é necessário que os desenvolvedores (ou modificadores)
    disponibilizem o **código fonte**!

--- .segue bg:red

<br><br><br>
## Atenção!
<br>
## Não confundir software **livre** com software **grátis**
<br>
## Livre como em “liberdade de expressão”, não grátis como “cerveja grátis”

---

## Software Livre

### Um software só é considerado livre quando é possível ter as 4 liberdades

0. Liberdade para usar o programa para qualquer propósito

1. Liberdade para estudar com o programa funciona, e modificá-lo para
    sua necessidade

2. Liberdade para redistribuir cópias (e ajudar o seu vizinho)

3. Liberdade para aprimorar o programa, e redistribuí-lo para que todos
    se beneficiem

---

## Software Livre

### Licenças livres

- GNU General Public License (GPL)

- BSD License

- Mozilla Public License

- MIT License

- Apache License

---

## Software Livre

### Exemplos de software livre que você já usa

- R!

- OpenOffice

- Firefox, Thunderbird

- Chromium (baseado no Google Chrome)

- LaTeX

---

## Software Livre

### Repositórios de software livre

- GitHub [http://github.com]()

- SourceForge [http://sourceforge.net]()

- Google Code [http://code.google.com]()

---

## Software Livre

### Quem usa software livre?

- Academia

- Indústria

- Governo

    - [http://www.softwarelivre.gov.br]()

    - [http://www.softwarepublico.gov.br]()

    - [https://www.serpro.gov.br]()

--- .segue bg:green
<br>
## Você!
<br>
## A internet e a WWW surgiram do mesmo movimento e princípios do software livre
<br>
## Hoje em dia a grande maioria dos sites usa o servidor Apache e banco de dados MySQL para funcionar

---

## Software Livre

### Vantagens do software livre

- Projetos colaborativos: pessoas com experiências e visões diferentes
    contribuem para o benefício comum

- Segurança: *Given enough eyeballs, all bugs are shallow*

- Qualidade: o que é melhor, 12 ou 1M desenvolvedores?

- Sem “caixa preta”: transparência

- Flexibilidade: você decide o que usar e quando usar

- E **também** é de graça!

---

## Software Livre

### Porque devo me importar?

- Por todas as vantagens acima

- Como cientistas

    - Devemos ser transparentes em nossas pesquisas

    - Temos que reportar aquilo que estamos fazendo

    - Temos que provar os resultados que obtemos

    - Nossa pesquisa tem que ser **reproduzível**
