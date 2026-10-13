# br-flags

Bandeiras do Brasil, das 27 unidades da federação e de 4.010 municípios brasileiros, com o arquivo de cada uma escolhido pelo Wikidata e baixado do Wikimedia Commons.

## Estrutura

| Caminho | Conteúdo |
|---|---|
| `BR.svg`, `BR-mini.webp` | bandeira do Brasil (original do Commons em SVG e miniatura) |
| `BR-brasao.svg`, `BR-brasao-mini.webp` | brasão de armas do Brasil |
| `EX.svg`, `EX-mini.webp`, `EX-brasao.svg`, `EX-brasao-mini.webp` | ONU, usada como "exterior" |
| `uf/XX.svg`, `uf/mini-XX.webp` | 27 bandeiras estaduais e a do DF, pela sigla da UF |
| `municipio/{código IBGE}.webp` | 4.010 bandeiras municipais, com até 512 px de altura |
| `municipio-mini/mini-{código IBGE}.webp` | 4.011 miniaturas municipais |
| `municipios.tsv` | uma linha por bandeira municipal: código IBGE, UF, nome, slug, arquivo, miniatura, licença, autor e fonte no Commons; depois de uma linha em branco, os municípios sem bandeira |
| `municipios-sem-bandeira.md` | os municípios sem bandeira, por UF, e o motivo |

As miniaturas cabem numa caixa de 32×32 px. Tudo é WEBP, fora os SVG originais do Brasil, da ONU e das UFs.

## Como usar

Pelo jsDelivr, com o código IBGE de 7 dígitos:

```
https://cdn.jsdelivr.net/gh/A78JR/br-flags@main/municipio/3550308.webp
https://cdn.jsdelivr.net/gh/A78JR/br-flags@main/municipio-mini/mini-3550308.webp
https://cdn.jsdelivr.net/gh/A78JR/br-flags@main/uf/SP.svg
```

Município sem arquivo não tem bandeira no Wikidata (ou ela não pôde ser baixada).

## Licenças

Cada bandeira mantém a licença do seu arquivo no Wikimedia Commons. A licença, o autor e a página de origem de cada bandeira municipal estão no `municipios.tsv` e também nos metadados EXIF e XMP do próprio WEBP. A conversão para WEBP é de A78JR.
