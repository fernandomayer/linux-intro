# Introdução ao uso do Linux

Este branch é o repositório dos slides utilizados no curso.

Os slides foram criados com o pacote [Slidify](http://www.slidify.org) do R. É
necessário instalar a versão em desenvolvimento deste pacote disponível
no [GitHub](https://github.com/ramnathv/slidify/tree/dev):

```r
require(devtools)
install_github("slidify", "ramnathv", ref = "dev")
install_github("slidifyLibraries", "ramnathv", ref = "dev")
```
Após a instalação, e com estes arquivos devidamente baixados:

```r
require(slidify)
slidify("index.Rmd")
```

O resultado final é o arquivo `index.html`, em HTML5, que pode ser
aberto diretamente no navegador (preferencialmente o Chromium).

As modificações devem ser feitas no arquivo `Rmd` que é uma extensão da
linguagem Markdown para o R. A interpretação será feita pelo pacote
[`knitr`](http://yihui.name/knitr) (que também deve estar instalado).

Para publicar é necessário um repositório próprio no GitHub. Neste caso,
o comando utilizado foi

```r
publish("linux-intro", "fernandomayer", host = "github")
```

Note que para publicar no GitHub, o repositório já deve estar
devidamente configurado e no branch `gh-pages`.

Com o Slidify também é possível publicar no [Dropbox](http://www.dropbox.com) e
no [RPubs](http://rpubs.com) - veja `?publish` para isso.

**Contribuições serão sempre bem-vindas**. A melhor forma de contribuir
  é dando um fork nesse repositório e enviar suas contribuições por
  *pull request*. Para uma rápida introdução ao git e GitHub veja o
  [git-rautu](https://github.com/fernandomayer/git-rautu).
  
## Licença

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.pt_BR"><img alt="Licença Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br />Esta obra foi licenciada sob uma Licença <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.pt_BR">Creative Commons Atribuição-CompartilhaIgual 3.0 Não Adaptada</a>.
