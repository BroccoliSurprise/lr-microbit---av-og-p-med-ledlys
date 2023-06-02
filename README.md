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

