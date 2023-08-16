# control flow

```py
def control_flow(value):
    if value:
        # if the value is truthy
        print("yep!")
    else:
        # if the value is falsy
        print("nope!")

control_flow(False)
# "nope!"
control_flow(None)
# "nope!"
control_flow(True)
# "yep!"
control_flow("")
# "nope!"
control_flow(0)
# "nope!"
control_flow("0")
# "yep!"
```

```py

dog = "me"

if dog == "friendly":

    owner = "say hi"

elif dog == "thief":

    owner = "bark"
else:

    owner = "stay calm boy"

print(owner)

```

```py

def control_flow (value):

    if value:

        print("yup")

    else:

        print("nope")


control_flow(1)      / control_flow(0)

# yup

# nope

```

## Conditional Expression

Here we use the `tenary operator` used to show truthiness of complex statement in a single line.

```py
age = 1

is_baby = 'baby' if age < 2 else 'not a baby'

or

name = "Sam"

student = "yes" if name == "Tasha" else "not a student"

print(student)

```

This is the equivalent of the following `if/else` statement:

```py
age = 1
if age < 2:
  is_baby = 'baby'
else:
  is_baby = 'not a baby'
```

## try/except statemen

Exceptions are a type of error that we can intercept so that our Python application can continue to run. 

`try/except`- allows us to perform interceptions.

```py
def divide(num1, num2):
    try:
        quotient = num1 / num2
        print(quotient)
    except ZeroDivisionError:
        print("Error: num2 cannot be equal to 0")
    except TypeError:
        print("Error: input must be of type int or float")
    finally:
        print("Isn't division fun?")

divide(6,3)        

# 2.0
# Isn't division fun?
```

# Dictionary Mapping

Here we use `match/case` to avoid repetition

```py

dog = "cuddly"

if dog == "hungry":
    owner = "Refilling food bowl."
elif dog == "thirsty":
    owner = "Refilling water bowl."
elif dog == "playful":
    owner = "Playing tug-of-war."
elif dog == "cuddly":
    owner = "Snuggling."
else:
    owner = "Reading newspaper."

```

`mapping`

```py
dog = "cuddly"

dict_map = {
    "hungry": "Refilling food bowl.",
    "thirsty": "Refilling water bowl.",
    "playful": "Playing tug-of-war.",
    "cuddly": "Snuggling.",
}

# Remember that a dictionary's .get() method lets us set a default value!
owner = dict_map.get(dog, "Reading newspaper.")


or


dog = "friendly"

my_dog = {

    "friendly": "say hey",
    "thief": "bark",

}

me = my_dog.get(dog,"walk away")

print(me)
```