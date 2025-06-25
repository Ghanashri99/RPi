import RPi.GPIO as GPIO
import time 

GPIO.setmode(GPIO.BOARD)

led = 3

GPIO.setup(led, True)

while True:
  GPIO.output(led, True)
  time.sleep(1)
  GPIO.output(led, False)
  time.sleep(1) 
