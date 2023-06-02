#  Lær micro:bit - Av og på med LEDlys

## Steg 1 

Last ned dette programmet til micro:biten og se hva som skjer med det røde LEDlyset

```template
basic.forever(function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
    basic.pause(500)
    pins.digitalWritePin(DigitalPin.P0, 1)
    basic.pause(500)
})
```

## Steg 2 
Klarer du å få den røde, gule og grønne LEDen til å blinke som et trafikklys?

## Steg 3
Avansert utfordring:
Klarer du å få lysene til å blinke gradvis lysere og mørkere? Trykke på lyspæren hvis du trenger et hint.

```blocks
basic.forever(function () {
for (let indeks = 0; indeks <= 100; indeks++) {
    pins.analogWritePin(AnalogPin.P0, indeks)
}
})

```


```ghost
basic.showNumber(0)
basic.showIcon(IconNames.Heart)
basic.showLeds(`
    . . . . .
    . . . . .
    . . . . .
    . . . . .
    . . . . .
    `)
basic.showString("Hello!")
basic.pause(randint(0, 10))
pins.analogWritePin(AnalogPin.P0, 1023)
for (let indeks = 0; indeks <= 4; indeks++) {
	
}
```


> Åpne denne siden på [https://broccolisurprise.github.io/lr-microbit---av-og-p-med-ledlys/](https://broccolisurprise.github.io/lr-microbit---av-og-p-med-ledlys/)

## Bruk som utvidelse

Dette kodeområdet kan bli lagt til som en **utvidelse** i MakeCode.

* åpne [https://makecode.microbit.org/](https://makecode.microbit.org/)
* klikk på **Nytt prosjekt**
* klikk på **Utvidelser** i menyen under tannhjulet
* søk etter **https://github.com/broccolisurprise/lr-microbit---av-og-p-med-ledlys** og importér

## Rediger dette prosjektet ![Build status badge](https://github.com/broccolisurprise/lr-microbit---av-og-p-med-ledlys/workflows/MakeCode/badge.svg)

For å redigere dette kodeområdet i MakeCode.

* åpne [https://makecode.microbit.org/](https://makecode.microbit.org/)
* klikk på **Importer** og så på **Importér URL**
* lim inn **https://github.com/broccolisurprise/lr-microbit---av-og-p-med-ledlys** og klikk på importér

## Blocks preview

This image shows the blocks code from the last commit in master.
This image may take a few minutes to refresh.

![A rendered view of the blocks](https://github.com/broccolisurprise/lr-microbit---av-og-p-med-ledlys/raw/master/.github/makecode/blocks.png)

#### Metadata (brukes for søk, visualisering)

* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
