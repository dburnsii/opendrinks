Images:
 - Must be 500x500 px and in jpg format
 - Must be named the same name as an existing drink
 - Must be licensed under a Creative Commons License and listed in the `credits.txt` file

Ingredients:
 - name (String): Name of the ingredient (required: true)
 - measure (String): Method of measuring this ingredient. The Bartender will assume it can pour anything measured in mL, even though this may not be the case in real life. (required: true)
 - carbonated (Boolean): Determines if this ingredient is carbonated. The Bartender has to handle carbonated beverages differently, so this value is important. (required: true)

Recipes:
 - name (String): Name of the drink (required: true)
 - description (String): Description of the drink (required: false)
 - alias (Array(String)): Other names a user might search to find this recipe
 - image (String): Filename for the image for this recipe, resides in the `images` folder
 - ingredients (Array):
  - ingredient (String): Name of the ingredient (required: true)
  - quantity (Float): Quantity of ingredient (required: true)
  - required (Boolean): Whether or not the ingredient is required to make the drink (required: true)
