# AlphaPwners Cookies
### by team AlphaPwners

```Python
# Import elements
import ingrediends from fridge as ing
import microwave, bowl, utils from kitchen
import units from metrics as u
import time

# Add ingredients into bowl with units multipler to calculate correct amount
bowl.add(ing.SUGAR, 4 * u.TABLESPOON)
bowl.add(ing.FLAVOUR, 4 * u.TABLESPOON)
bowl.add(ing.CACAO, 2 * u.TABLESPOON)
bowl.add(ing.OIL, 1 * u.TABLESPOON)
bowl.add(ing.MILK, 3 * u.TABLESPOON)
bowl.add(ing.EGG, 1 * u.UNIT)
bowl.add(ing.BAKING_POWDER, 0.25 * u.TEASPOON)
bowl.add(ing.SALT, 0.05 * u.TEASPOON)

# Mixing and baking
bowl.mix_together()
while not bowl.getCake().isBaked():
	# Its default 600W microwave, for other wattage, use third parameter, eg:
	# microwave.bake(bowl, 30 * u.SECONDS, 750 * u.WATS)
	microwave.bake(bowl, 30 * u.SECONDS) 
	
# TODO: Safety check for hot bowl, already instad i use sleep
time.sleep(30)

# Cutting and preparing cookies
cake = bowl.getCake()
cookies = [utils.cut_shape(layer) for layer in cake]

# Cleaning whole stuff
utils.clean_whole_kitchen()
utils.prevent_for_eat_before_xmas()

print "Happy christmas from AlphaPwners!"
```

The making of: https://streamable.com/088yk

![Cookies](cookies_AlphaPwners.jpg)
![Evaluation](evaluation_AlphaPwners.jpg)
