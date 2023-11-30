# SYSA-APPEdit with the Docs app
Make tweaks, leave comments, and share with others to edit at the same time.
NO THANKSUSE THE APP

SYSA APP MVP specification
SYSA APP

An app that generates based on the ingredients you select and saves old recipes.


Team members

Sali Sohkohlo

Sylvia Ogbonna


Technologies

HTML CSS Javascript

NPM  alternatives are NGX

Python alternatives are Javascript


Challenges

SYSA is a project that helps keep track of the users healthy diet, and generate healthy meal options.

SYSA will not keep track of your weight, or help you on a weight loss jpurney.

SYSA users are for dieters between the ages of 25 - 50 including male and female.

SYSA is not dependent on a certain locale.


Risks

The risks could include:

Wrong recipes and measurements
Alternatives will be a disclaimer.

The non-technical risks are:

Reliability on the app.

Infrastructure

The main will be created by either of the team, both parties will work in branches and once the work is done and approved, will be merged.


Data will be gotten via an existing API.


Testing and automation will be considered later.


Existing solutions

DishGen - DishGen uses AI to generate recipes by tailoring the ingredients provided to suggest available recipes.


We intend to reimplement the app to work on the healthy meal options to manage high sugar and carb foods.


Architecture





API and Methods

Edamam Recipe search API.


https://www.edamam.com/#!/Recipe_Search/get_api_recipes_v2

Recipe Search
GET /api/recipes/v2


https://www.edamam.com/#!/Search_by_recipe_URI/get_api_recipes_v2_by_uri

Search by recipe URI

GET /api/recipes/v2/by-uri


https://www.edamam.com/#!/Specific_Recipe_Info/get_api_recipes_v2_id

Specific Recipe Info

GET /api/recipes/v2/{id}


Data Model


recipes Table:

recipe_id (Primary Key)
title
instructions
Image_url

ingredients Table:

ingredient_id (Primary Key)
name


recipe_ingredients Table:

recipe_id
ingredient_id
quantity
unit



User story


User Story 1: Ingredient Input

A user interested in discovering recipes with my available ingredients,


I want to be able to input a list of ingredients easily,


So that the app can generate recipe suggestions based on what I have on hand.


Acceptance Criteria:


The app should have a dedicated page or section for ingredient input.

I should be able to manually enter ingredients in a text field.

/*Alternatively, I want the option to use a barcode scanner to input packaged

items. */

The app should validate and handle common variations and synonyms of ingredient names.

After entering the ingredients, I should have the option to proceed to recipe suggestions.


User Story 2: Recipe Suggestions

A user seeking cooking inspiration,


I want to receive recipe suggestions based on the ingredients I've provided,


So that I can discover new and interesting dishes to prepare.


Acceptance Criteria:


After entering ingredients, the app should display a list of recipe suggestions.

Each recipe suggestion should include a title, image, list of ingredients, and detailed instructions.

If a suggested recipe requires additional ingredients, the app should clearly indicate what is missing.

I should be able to save recipes I'm interested in for future reference.

The app should provide diverse recipe suggestions covering various cuisines and difficulty levels.



User Story 3: Search and Filter

A user with specific preferences,


I want to be able to search and filter recipe suggestions,


So that I can find recipes that match my dietary preferences, cuisine preferences, or cooking time constraints.


Acceptance Criteria:


The app should have a search bar allowing me to search for specific recipes or ingredients.

I should be able to filter recipe suggestions based on dietary preferences (e.g., vegetarian, gluten-free).

Filtering options should include cuisine types (e.g., Italian, Asian) and preparation time.

The search and filter functionality should be intuitive and user-friendly.



User Story 4: Save and View Saved Recipes

A user who wants to keep track of favorite recipes,


I want to save and view recipes for future reference,


So that I can easily access the recipes I enjoy.


Acceptance Criteria:


Each recipe suggestion should have a "Save" button for quick bookmarking.

There should be a dedicated section in the app to view and manage saved recipes.

I should be able to remove recipes from my saved list.



User Story 5: User-Friendly Interface

A user looking for a hassle-free experience,


I want the app to have an intuitive and visually appealing interface,


So that I can easily navigate through the app and enjoy the recipe discovery process.


Acceptance Criteria:


The app should have a clean and organized layout with easily identifiable sections.

Navigation should be straightforward, with clear labels and minimal complexity.

The user interface should be responsive and work seamlessly on both mobile and web platforms.


Mock up

Link provided below.

https://whimsical.com/sysa-FNbgBy4VUWRrJrCQ6SG5SB

