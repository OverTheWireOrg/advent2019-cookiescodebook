# AlphaPwners Cookies
### by team AlphaPwners

```Python
# Import elements
import ingrediends from fridge as ing
import microwave, bowl, utils from kitchen

# Add ingredients into bowl
bowl.add(ing.SUGAR, 4)
bowl.add(ing.FLAVOUR, 4)
bowl.add(ing.CACAO, 2)
bowl.add(ing.OIL, 1)
bowl.add(ing.MILK, 3)
bowl.add(ing.EGG, 1)
bowl.add(ing.BAKING_POWDER, 0.25)
bowl.add(ing.SALT, 0.05)

# Mixing and baking
bowl.mix_together()
microwave.bake(bowl, 150)

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
