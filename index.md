---
title       : Introdução ao uso do Linux
subtitle    : Conceitos básicos e instalação
author      : Fernando de Pol Mayer & Luiz Ricardo Nakamura
date        : 2013-09-02
job         : ESALQ/USP - 02 e 03 de Setembro, 2013
logo        : Tux.svg
license     : by-sa
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
assets      :
  css: "http://netdna.bootstrapcdn.com/font-awesome/3.2.1/css/font-awesome.css"
---

<!-- Algumas modificacoes necessarias enquanto o codigo do Slidify esta -->
<!-- em desenvolvimento -->
<!-- Para as marcacoes funcionarem -->
<style>
strong {
	font-weight: bold;
}
em {
	font-style: italic
}
</style>
<!-- FIM -->

<br><br><br>
### Slides disponíveis em [http://fernandomayer.github.io/linux-intro]()

### Feito com [Slidify](http://slidify.org)

### Melhor visualizado com [Chromium](http://www.chromium.org) (ou [Google Chrome](https://www.google.com/chrome))

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

<i class="icon-unlock icon-4x pull-left icon-muted"></i>

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

1. Liberdade para estudar como o programa funciona, e modificá-lo para
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

- Google Chrome (no Linux é Chromium)

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
## Hoje em dia a grande maioria dos sites usa o servidor Apache e banco de dados POSTGRES para funcionar

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

---

## Software Livre

### Ciência (Estatística) aberta

Um exemplo: [FOAS](http://www.foastat.org)
<br>
<div class="centered">
<img src="assets/img/foas.png" width=80%/>
</div>

--- .segue .nobackground .dark

## O Sistema Operacional GNU/Linux

--- #myslide

<script>
$('#myslide').on('slideenter', function(){
  $(this).find('article')
    .append('<iframe width="640" height="360" src="//www.youtube.com/embed/yVpbFMhOAwE?rel=0" frameborder="0" allowfullscreen></iframe>')
});
$('#myslide').on('slideleave', function(){
  $(this).find('iframe').remove();
});
</script>

---

## Sistema Operacional

- É um conjunto de programas que fazem a interface entre o usuário e o
  *hardware*

- Sua principal função é o gerenciamento de recursos e periféricos,
  interpretação de mensagens e execução de programas

- Um SO pode ser dividido em duas partes:
	- **Núcleo** ou **kernel** desempenha as funções vitais do sistema
        (baixo-nível) $\rightarrow$ **Linux**
	- **Concha** ou **Shell** é a interface entre o usuário e o
        kernel. Pode ser em um formato "cru" como a linha de comando ou
        mais amigável com janelas gráficas $\rightarrow$ **GNU**

- O conjunto de kernel Linux e dos programas GNU é o sistema operacional
  que chamamos de **GNU/Linux** (ou simplesmente Linux)


---

## Linux

<!-- ### Histórico -->
<!-- - **1969-1973** Ken Thompson e Dennis Ritchie (Bell Labs) $\rightarrow$ -->
<!--     Unix (fechado e caro) -->
<!-- - **1987** Andrew Stuart Tanenbaum $\rightarrow$ Minix (aberto) -->
<!-- - **1991** Linux Torvals $\rightarrow$ Linux -->

### Principais características

- Livre e desenvolvido voluntariamente por programadores experientes,
  hackers, e contribuidores espalhados ao redor do mundo

- Convive pacificamente com outros sistemas operacionais no mesmo
  computador (embora não seja a melhor opção...)

- Multitarefa e multiusuário

- Modular: carrega apenas o necessário e libera memória após a
  utilização

- Não há a necessidade de reiniciar o sistema após a modificar alguma
  configuração ou instalar programas (apenas na atualização de kernel)

---

## Linux

### Principais características

- Roda confortavelmente em sistemas de baixo desempenho (processadores
  antigos, pouca memória RAM)

- **Não é vulnerável à vírus!** Devido à separação de privilégios clara
    entre usuário e administrador, vírus possuem uma ação muito
    limitada, por isso são inúteis. (Esqueça o anti-vírus!)
	
- Suporte completo e nativo a diversos dispositivos de comunicação (USB,
  Bluetooth, ...)
	  - Raramente serão necessários drivers externos (com excessão de
        tecnologias muito novas)

- Os sistemas de arquivos usados pelo GNU/Linux (Ext3, reiserfs, ...)
  organizam os arquivos de forma inteligente evitando a
  **fragmentação**, tornando um poderoso sistema para aplicações
  exigentes e gravações intensivas. (Esqueça o desfragmentador!)

---

## Linux

### Distribuições do Linux

- Devido à sua liberdade, um grupo de pessoas, empresa ou
  organização pode decidir distribuir uma versão do Linux com diferentes
  características
	  - Facilidade de uso
	  - Foco em desempenho
	  - Agrupar programas de interesse (programação, edição gráfica,
        ...)

- Cada **distribuição** tem uma característica própria como o sistema de
  instalação, objetivo, ..., embora todas apresentem a mesma estrutura
  básica do Linux


---

## Linux

### Distribuições do Linux

Figura com vários logos

---

## Linux

### GUIs (Graphical User Interface)

Diversas cascas (*shell*) existem para o Linux. Algumas das principais
são:
- [Gnome](http://www.gnome.org)
- [KDE](http://www.kde.org)
- [XFCE](http://www.xfce.org)
- [Unity](https://unity.ubuntu.com)

Além, é claro, do **terminal**, onde você possui uma interação mais
"direta" com o kernel (veremos adiante).

Aqui você também tem a opção de escolha!

---

## Linux

### Estrutura básica de diretórios

**O mais importante:** no Linux os diretórios são separados por `/` e
  não por `\` como no Windows
- Além disso, uma `/` (barra sozinha) tem um significado especial: é a
  **raíz de todo o sistema**, ou seja, todos os diretórios começam a
  partir dela.

Alguns dos principais diretórios são:
- `/bin` e `/sbin`: arquivos executáveis de programas
- `/etc`: arquivos de configuração
- `/home`: arquivos pessoais do usuário

--- .segue .nobackground .dark

## Ubuntu

---

## Ubuntu

### Origem

- Termo Africano para "humanidade para os outros"

- Uma distribuição Linux baseada na simplicidade, usabilidade e fácil
  instalação

- Baseado na distribuição **Debian**, e patrocinada pela empresa Canonical

- Hoje é mantida pela (ampla) comunidade, apoiada pela Canonical

---

## Ubuntu

### Características

- Novas versões lançadas a cada 6 meses (em maio e outubro)
	- Suporte (atualizações) mantido por 9 meses nas versões normais, e
      por 5 anos nas versões LTS (Long Term Support)

- Central de programas com XXXX pacotes disponíveis

- Funciona "Live": através de um pen-drive ou DVD, sem necessidade de
  instalação

- Diversos "sabores":
	- [Edubuntu](http://www.edubuntu.org)
	- [Xubuntu](http://www.xubuntu.org)
	- [Ubuntu GNOME](http://ubuntugnome.org)
	- [Ubuntu Studio](http://ubuntustudio.org)

