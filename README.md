# Python-Resturaunt-Project
print("""Konchada Restuarant
-----------------
Menu
-----------------""")
print("""APPETIZERS
1.Samosas 5.50
2.Chicken 65 6.50
3.Veg Pakora 4.25
-----------------""")
print("""CURRIES
1. Chicken Curry 14.25
2. Veg curry 16.25
3. Mutton curry 15.25
4. Fish curry 15.25""")
print("""-----------------""")
print("""BIRYANIS
1. Vijaywada Chicken Biryani 17.50
2. Mutton Biryani 15.75
3. Veg Biryani 16.75
4. Egg Biryani 14.50
-----------------""")

appetizer_price = 0
appetizer_order = input("What Appetizer would you like today? ")
if appetizer_order.lower() == "samosas":
   appetizer_price = 5.50
if appetizer_order.lower() == "chicken 65":
   appetizer_price = 6.50
if appetizer_order.lower() == "Veg Pakora":
   appetizer_price = 5.50
if appetizer_order.lower() == "none" or appetizer_order.lower() == "nothing" or appetizer_order.lower() == "":
   appetizer_price = 0
print(" ")
curry_price = 0
curry_order = input("What Curry would you like today? ")
if curry_order.lower() == "chicken curry":
  spice_level = input("Mild, Hot, or Very Hot? ")
  curry_price = 14.25
if curry_order.lower() == "veg curry":
  spice_level = input("Mild, Hot, or Very Hot? ")
  curry_price = 16.25
if curry_order.lower() == "mutton curry":
  spice_level = input("Mild, Hot, or Very Hot? ")
  curry_price = 15.25
if curry_order.lower() == "fish curry":
  spice_level = input("Mild, Hot, or Very Hot? ")
  curry_price = 15.25
if curry_order.lower() == "none" or curry_order.lower() == "nothing" or curry_order.lower() == "":
  curry_price = 0
  spice_level = ""
print(" ")
biryani_price = 0
biryani_order = input("What Biryani would you like today? ")
if biryani_order.lower() == "vijaywada chicken biryani":
   biryani_price = 17.50
if biryani_order.lower() == "mutton biryani":
   biryani_price = 15.75
if biryani_order.lower() == "veg biryani":
   biryani_price = 16.75
if biryani_order.lower() == "egg biryani":
   biryani_price = 14.50
if biryani_order.lower() == "none" or biryani_order.lower() == "nothing" or biryani_order.lower() == "":
   biryani_order = ""
   biryani_price = 0
print(" ")
print("Your order is " + str(appetizer_order.title()) + ", " + str(curry_order.title()) + "(" + str(spice_level.title()) + "), " + str(biryani_order.title()))
print("Your total is: $" + str(float(appetizer_price) + float(curry_price) + float(biryani_price)))
