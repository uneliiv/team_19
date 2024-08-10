
# teamwork-01.08.-Postman

TASK FOR TEAMWORK : 

1. Send a POST request

public ResultItem sendItem(Item item)

2. You should send one object and receive a different object with different data

3. Test it out POSTMAN
------------------------------
```java
 @PostMapping("/makeMeal")
    public Meal makeMeal(@RequestBody Ingredients ingredients) {
        if (ingredients.ingredient1.equals("bread") && ingredients.ingredient2.equals("cheese")
                && ingredients.ingredient3.equals("meat")) {
            var meal = new Meal();
            meal.name = "Burger";
            return meal;
        }
        return null;
    }
}
```

```java
package com.datorium.Datorium.API;

public class Ingredients {
    public String ingredient1;
    public String ingredient2;
    public String ingredient3;
}
```

```java
package com.datorium.Datorium.API;

public class Meal {
    public String name;
}
```

RESULT :

![image](https://github.com/user-attachments/assets/70704962-e2e8-4de3-af5b-a5702a87ea95)


