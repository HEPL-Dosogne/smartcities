# LED 3 états
Dans ce premier exercice nous allons changer l'état de d'une led grâce à un bouton poussoir. Lors de la première pression, la led clignotera. Lorsqu'on appuie une deuxième fois sur le bouton, la led clignote plus vite et un troisième pression coupe la led.

Voici le code:

## Dosogne Guillaume 02/24

import machine
import utime

Button = machine.Pin(16, machine.Pin.IN)
LED = machine.Pin(18, machine.Pin.OUT)
val = 0

def blink():
    LED.value(1)
    utime.sleep(0.5)
    LED.value(0)
    utime.sleep(0.5)

def blinkFast():
    LED.value(1)
    utime.sleep(0.1)
    LED.value(0)
    utime.sleep(0.1)

def LedOff():
    LED.value(0)
    global val
    val = 0
    utime.sleep(1)

def etat(pin):
    global val
    val = val + 1
    if val > 3:
        val = 1
    utime.sleep(0.2)

Button.irq(trigger=machine.Pin.IRQ_FALLING, handler=etat)

while True:
    if val == 1:
        blink()
    elif val == 2:
        blinkFast()
    elif val == 3:
        LedOff()



