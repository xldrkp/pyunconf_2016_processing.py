% Processing.py and Arduino
% Axel Dürkop, TUHH
% Pyunconf Sep 10, 2016

# Learning Python with Processing

## Processing

- https://processing.org/
- IDE for easily developing artistic programms
- Code usually being compiled to Java

------

![Processing IDE](./abb/ide.png)

## Processing.py

- Python is a *mode* in Processing

![Installing Python mode](./abb/mode-installieren-1.png)

## (Almost) the best of two worlds

- Lots of Processing libraries can be used
- Main Python packages can be used

-----

![Choosing a library](./abb/lib-library-hinzufuegen.png)

-----

![Install it, if not already](./abb/lib-libraries-laden.png)

------

![Import it](./abb/lib-importiert.png)


## Processing.py Example

![The two main functions](./abb/Auswahl_106.png)

# Arduino

## Hardware

![Arduino Uno Board, Arduino Uno by [Snootlab](https://www.flickr.com/photos/snootlab/) [CC-BY 2.0](https://creativecommons.org/licenses/by/2.0/)](./abb/arduino-uno-flickr-snootlab.jpg)

------

![Arduino IDE](./abb/arduino_ide.png)

## Blink

```Java
byte led = 13;

void setup() {
  pinMode(led, OUTPUT);
}

void loop() {
  digitalWrite(led, HIGH);  
  delay(1000);         
  digitalWrite(led, LOW);
  delay(1000);
}
```

## Blink

![After compiling and uploading](./abb/blink.gif)

## Firmata

> "Firmata is a protocol for communicating with microcontrollers from software on a host computer. (https://github.com/firmata/arduino)"

- **StandardFirmata** is a preinstalled library in the Arduino IDE

## Firmata

- Once transfered like a normal sketch to the Arduino
- Serial communication (via USB) from the host computer using Processing.py

-------

![Communication with Arduino](./abb/workflow.png)

## API

- `list()`
- `pinMode(pin, mode)`
- `digitalRead(pin)`
- `digitalWrite(pin, value)`
- `analogRead(pin)`
- `analogWrite(pin, value)`
- `servoWrite(pin, value)`

# Why not PyGame?

## PyGame

First line is the import of a library

```Python
import sys, pygame
pygame.init()
```

## Processing.py

First success comes with one, two line(s) of code

```Python
def draw():
  ellipse(mouseX, mouseY, 20, 20)
```

## Links

- http://www.python-processing-arduino.de/
- axel.duerkop@tuhh.de
- @xldrkp
- github.com/xldrkp
