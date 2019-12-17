# Chocolate Chip Cookies
### by team WeAreScientists

```python
import RetardUnits
import human
from datetime import datetime, timedelta
from siemens import oven
from wmf import bowl, mixer, bakingpan
from kitchen import parchmentpaper, rum

cookie_size = RetardUnits.tablespoon(2) # size of one cookie

oven = Oven()
bakingpan = Bakingpan()

Rum().pour(shots=1).drink()

oven.preheat(RetardUnit.fahrenheit(375))
bakingpan.max_room = 6 # max room for cookies
bakingpan.apply(Parchmentpaper().get_sheets(1))

Rum().pour(shots=1).drink()

dryBowl = Bowl({
    "all_purpose_flour": RetardUnits.cup(3),
    "baking_soda": RetardUnits.teaspoon(1),
    "baking_powder": RetardUnits.teaspoon(0.5),
})

butterBowl = Bowl({
    "salted_butter": RetardUnits.cup(1),
    "white_sugar": RetardUnits.cup(1),
    "brown_sugar": RetardUnits.cup(1),
    "large_eggs": 2,
    "vanilla_extract": RetardUnits.teaspoon(2)
})

Rum().pour(shots=2).drink()

butterBowl.mix_with(Mixer, [dryBowl, {"chocolate_chips": RetardUnits.cup(2)}])

Rum().pour(shots=3).drink()

if cookie_size > 0 and not butterBowl.empty():
    raw_cookie = roll_cookie(cookie_size)
    if bakingpan.check_room():
        bakingpan.apply(raw_cookie)

Rum().pour(shots=5).drink()

cookies = oven.bake(bakingpan, until=datetime.now() + timedelta(minutes=8) )

Rum().pour(shots=8).drink()

try
    human.consume(cookies)
except HumanScream:
    print("Watch it, cookies are hot")

print("""
    Nutrition Facts (1 Cookie)
    Calories 263.4 Calories from Fat 113

    % Daily Value*
    Total Fat 12.6g 19%
    Cholesterol 31.6mg 11%
    Potassium 115.4mg 3%
    Total Carbohydrates 41.2g 14%
        Dietary Fiber 1.4g 6%
        Sugars 25.5g
    Protein 2.7g 5%
    Vitamin A 5.2%
    Calcium 2.3%
    Iron 7%
""")
```

The making of: https://youtu.be/dQw4w9WgXcQ

![Cookies](cookies_WeAreScientists.jpg)
![Evaluation](evaluation_WeAreScientists.jpg)
