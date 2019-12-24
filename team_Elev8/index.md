# Chocolate Chip Christmas Cookies
### by team Elev8

#include <recipe_base.h>
#include <kitchen_utils.h>
#include <ingredients.h>

 

int main() {
    Oven *oven = allocate_oven();
    Bowl *bowl1 = allocate_bowl();
    Bowl *bowl2 = allocate_bowl();
    Surface *workarea = allocate_surface();
    Bakingtray *tray = allocate_bakingtray(INCLUDE_SILICONE_MAT);

    preheat(oven, 375, FARENHEIT);

    add_to_bowl(bowl1,ingredient("flour",2.25, CUP);
    add_to_bowl(bowl1,ingredient("baking soda",1, TSP);
    add_to_bowl(bowl1,ingredient("salt",1, TSP);
    mix_contents(bowl1);

    add_to_bowl(bowl2,ingredient("melted butter",1, CUP);
    add_to_bowl(bowl2,ingredient("granulated sugar",0.75, CUP);
    add_to_bowl(bowl2,ingredient("brown sugar",0.75, CUP);
    add_to_bowl(bowl2,ingredient("vanilla",1, TSP);
    add_to_bowl(bowl2,ingredient("egg",1, PIECE);
    add_to_bowl(bowl2,ingredient("egg_yolk",1, PIECE);
    mix_contents(bowl2);

    add_to_bowl(bowl2,ingredient(bowl1,.5, PIECE);
    mix_contents(bowl2);

    add_to_bowl(bowl2,ingredient(bowl1,.5, PIECE);
    mix_contents(bowl2);

    add_to_bowl(bowl2,ingredient("chocolate chips",2, CUP);
    mix_contents(bowl2);

    add_to_bowl(bowl2,ingredient("christmas love",2, CUP);
    mix_contents(bowl2);

    refridgerate(bowl2, 60, MIN);
	spread_on_surface(workarea, get_contents(bowl2));

    while(!is_empty(workarea) && !is_full(tray)) {
        move(scoop_cookie_dough(workarea), tray);
    }

    move(tray, oven);

    sleep(600);

    empty_into(tray, cookiejar); 

    clean(bowl1);
    clean(bowl2);
    clean(workarea);
    clean(cooldown(tray));
    clean(cooldown(oven));

    return HAPPY_AND_SATISFIED;
}
```

The making of: https://www.youtube.com/watch?v=VaT3qsoHPQ8

![Cookies](cookies_Elev8.jpg)
![Evaluation](evaluation_Elev8.jpg)
