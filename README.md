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

Para publicar é necessário um repositório próprio no GitHub. Neste caso,
o comando utilizado foi

```r
publish("linux-intro", "fernandomayer", host = "github")
```

Note que para publicar no GitHub, o repositório já deve estar
devidamente configurado e no branch `gh-pages`.

Com o Slidify também é possível publicar no [Dropbox](http://www.dropbox.com) e
no [RPubs](http://rpubs.com) - veja `?publish` para isso.
