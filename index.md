---
title       : Introdução ao uso do Linux
subtitle    : Conceitos básicos e instalação
author      : Fernando de Pol Mayer
date        : 2013-09-02
job         : ESALQ/USP
logo        : Tux.svg
biglogo     : Tux.svg
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
assets      :
  css: "http://netdna.bootstrapcdn.com/font-awesome/3.2.1/css/font-awesome.css"
---

--- .segue .nobackground .dark

## Software Livre

--- &twocol

## Software Livre

Richard Stallman - Projeto GNU (1983)

*** =left

<div class="centered">
<img src="assets/img/RMS.jpeg" width=40%/>
</div>

*** =right

<div class="centered">
<img src="assets/img/GNU.png" width=40%/>
</div>

--- &twocol

## Software Livre

Linus Torvalds - Linux (1991)

*** =left

<div class="centered">
<img src="assets/img/LT.jpeg" width=40%/>
</div>

*** =right

<div class="centered">
<img src="assets/img/Tux.svg" width=40%/>
</div>

---

## Slide 0

O GNU

<div class="centered">
<img src="assets/img/GNU.png" alt="GNU" height=20% />
</div>


--- .nobackground .dark

## O Terminal

```{shell}
cd ~/Linux
```

--- &twocol

## Slide 0.0

O GNU

*** =left

* Item 1
* Item 2

*** =right

* Item 3


---

## Slide 1

Como fazer um block

```
fernando@kirk:~/GitHub/linux-intro$ ls
assets  index.html  index.md  index.Rmd  libraries
```

--- 

## Slide 2

Teste de texto

---

## Slide 3

Lista
* Item 1
* Item 2
    - Sub-item 1
    - Sub-item 2

---

## Slide 4

Um bloco com código do **R**


```r
rnorm(10)
```

```
##  [1]  0.07983  0.10391 -0.55007  0.72545  0.51363  2.10287 -0.47120
##  [8]  0.20636  0.02176  0.13725
```


---

## Slide 5

Mais um teste com block

> Bloco de texto

```
ls
```

Comandos úteis no terminal:
* `ls` para listar arquivos
* `cd` para mudar diretórios





