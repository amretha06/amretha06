 from gpiozero import Button

button = Button(21)

while True:
    print(button.is_pressed)
: while True:
    if button.is_pressed:
        print("Hello")
    else:
        print("Goodbye")
: while True:
    button.wait_for_press()
    print("Pressed")
    button.wait_for_release()
    print("Released")
: from gpiozero import Button,
: led = LED(25)
: while True:
    button.wait_for_press()
    led.on()
    button.wait_for_release()
    led.off()
 while True:
    led.on()
    button.wait_for_press()
    led.off()
    button.wait_for_release()
while True:
    led.blink()
    button.wait_for_press()
    led.off()
    button.wait_for_release()
 from gpiozero import Button,
 lights = TrafficLights(25, 8, 7)
 while True:
    button.wait_for_press()
    lights.on()
    button.wait_for_release()
    lights.off()
The TrafficLights interface is very
 while True:
    lights.blink()
    button.wait_for_press()
    lights.off()
    button.wait_for_release()
Add a buzzer
 from gpiozero import Button,
 buzzer = Buzzer(15)
 while True:
    lights.on()
    buzzer.off()
    button.wait_for_press()
    lights.off()
    buzzer.on()
    button.wait_for_release()
 while True:
    lights.blink()
    buzzer.beep()
    button.wait_for_press()
    lights.off()
    buzzer.off()
    button.wait_for_release()
from time import sleep
while True:
    lights.green.on()
    sleep(1)
    lights.amber.on()
    sleep(1)
    lights.red.on()
    sleep(1)
    lights.off()
: while True:
    button.wait_for_press()
    lights.green.on()
    sleep(1)
    lights.amber.on()
    sleep(1)
    lights.red.on()
    sleep(1)
    lights.off()

