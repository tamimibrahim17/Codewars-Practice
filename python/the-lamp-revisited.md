### The Lamp 
Define a class called Lamp. It will have a string attribute for color and boolean attribute, on, that will refer to whether the lamp is on or not. Define your class constructor with a parameter for color and assign on as false on initialize.

Give the lamp an instance method called toggle_switch that will switch the value of the on attribute.

Define another instance method called state that will return "The lamp is on." if it's on and "The lamp is off." otherwise.

### Solution
``` python
class Lamp(object):

	def __init__(self,color):
		self.color 	= color
		self.on 	= False

	def state(self):

		if self.on:
			return "The lamp is on."
		else:
			return "The lamp is off."

	def toggle_switch(self):

		if self.on:
			self.on = False
		else:
			self.on = True
```