# Typography

## Fonts

All text is set in *Source Sans Pro*—either `lighter`, `normal`, or
`bold`, or `italic` as style:

// Show font example
// TODO: This should maybe work without ``` as in example 2, 3, and 4.
```
@font-example lighter 30px Source Sans Pro, sans-serif
```

@font-example 30px Source Sans Pro, sans-serif

@font-example bold 30px Source Sans Pro, sans-serif

@font-example italic 30px Source Sans Pro, sans-serif


## Quotation Marks

We use the [Quotation-Marks Sass extension](http://quotation-marks.org) to localize quotations marks:

```
.formatted-text(***lang="en"***)
  %p
    The five boxing ***<q>***wizards***</q>*** jump quickly.

.formatted-text(***lang="de"***)
  %p
    Schweißgequält zündet Typograf ***<q>***Jakob***</q>*** verflixt öde Pangramme an.

.formatted-text(***lang="fr"***)
  %p
    Voyez le ***<q>***brick géant***</q>*** que j’examine près du wharf

.formatted-text(***lang="es"***)
  %p
    Benjamín pidió una ***<q>***bebida de kiwi y fresa***</q>***. Noé, sin vergüenza, la más exquisita champaña del menú.

.formatted-text(***lang="it"***)
  %p
    Qualche vago ***<q>***ione***</q>*** tipo zolfo, bromo, sodio
```

The language should be defined as `%html(lang="en")`.
