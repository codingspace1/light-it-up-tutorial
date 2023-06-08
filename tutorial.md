
# My Tutorial


## Step 1
Let's get started with the LEDs. First light up the LED at position (0,0). 
1. Drag the ``||led:led.plot(0,0)||`` function from LED section of the sidebar and drop in coding area.

```python
    Top left LED is at position(0,0)
    led.plot()
```

## Step 2
Now, light up the LEDs at positions (0,3) and (4,4) using ``||led:led.plot()||`` function.
Change the numbers in the ``||led:led.plot()||`` function to the position of LED you want to light up.


## Step 3
Since we know how to work with LEDs, let's display the letter **T** using the LEDs.
We need to light up the first row and the center column to display **T**.

```python
   led.plot(0,0)
   led.plot(1,0)
   led.plot(2,1)
```
## Step 4

Instead of manually lighting up the LEDs, let's use ``||basic:basic.show_leds()||`` function to display the letter **T**.
```python
basic.show_leds("""
# # # # #
. . . . .
. . # . .
. . . . .
. . . . .
""")
```
## Step 5

To display the scrolling text: 
1. We will use ``||basic:basic.show_string()||``function. This will show it only once.
2. Use ``||basic:basic.forever()||`` to display it continuously.

```python
def on_forever():
    basic.show_string("Hello!")
basic.forever(on_forever)

```
