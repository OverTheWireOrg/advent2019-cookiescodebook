# American Cookies
### By Datasnokmennene

```python
import drawer
import fridge
import time
import appliances	

def mix_butter_and_sugar(butter, sugar, vanilla, eggs):
    mix = appliances.mix(butter, sugar)
    mix.append(vanilla)
    mix.append(eggs)
    return mix

def dry_mix(flour, baking_soda, salt):
    mix = appliances.mix(flour, baking_soda, salt)
    return mix

def cut_chocolate(chocolate)
    bits = appliances.knife(chocolate)
    return bits

def main():
    # Set oven to 160 degrees celsius
    oven.temp(160)
    oven.mode(over_and_under_heat)

    # Making the dough
    # Add 250 grams of sugar and butter 1 table spoon of vanilla extract and 2 eggs
    dough = mix_butter_and_sugar(drawer.sugar*250, fridge.butter*250, drawer.vanilla*0.05, fridge.eggs*2)
    # Add 500 grams of flour, 1 teaspoon of baking soda and one teaspoon of salt
    dough += dry_mix(drawer.flour*500, drawer.baking_soda*0.05, drawer.salt*0.05)
    # Cut 200 grams of cholcolate
    dough += cut_chocolate(drawer.chocolate*200)

    # Adding to the oven
    while dough > 0:
        for i in appliances.baking_tray:
            appliances.baking_tray.append(dough)

        appliances.oven.add(tray)
        time.sleep(600)
        cookies = appliances.oven.remove(tray)
    
    
    drawer.box.add(cookies)
    print("Cookies finished")


main()
```

The making of: https://www.youtube.com/watch?v=38kgETqlO4w&feature=youtu.be

![cookies](cookies_datasnokmennene.jpg)
![evaluation](evaluation_datasnokmennene.jpg)
