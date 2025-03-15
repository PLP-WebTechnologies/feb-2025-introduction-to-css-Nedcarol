# Introduction to CSS

## Objectives
Link an external CSS file to an HTML document.
Apply basic styling using selectors.
Use colors, fonts, and spacing effectively.

## Instructions

Create a style.css file.
Apply CSS to a HTML page.
Style elements using:
Classes and IDs.
Color and typography.
Margins, paddings, and borders.

>[!NOTE]
>  - Include at least:
>  - Use of 3 selectors
>  - Style an image
>  - Margin, Padding & Borders
>  - Different font

# Tasks
 - Link an external CSS file.
 - Apply at least 3 different selectors.
 - Improve readability and aesthetics.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Delicious Pancake Recipe</title>
    <link rel="stylesheet" href="css/style.css">  <!-- External CSS Link -->
</head>
<body>
    <header>
        <h1 id="recipe-title">Delicious Pancakes</h1>
    </header>

    <div class="container">
        <!-- Recipe Image -->
        <img src="pancakes.jpg" alt="Fluffy Pancakes" class="recipe-image">

        <!-- Ingredients List -->
        <h2>Ingredients</h2>
        <ul class="ingredients-list">
            <li>1 cup flour</li>
            <li>2 tbsp sugar</li>
            <li>1 tsp baking powder</li>
            <li>½ tsp salt</li>
            <li>1 cup milk</li>
            <li>1 egg</li>
            <li>2 tbsp melted butter</li>
            <li>1 tsp vanilla extract</li>
        </ul>

        <!-- Instructions -->
        <h2>Instructions</h2>
        <ol class="instructions">
            <li>In a bowl, mix flour, sugar, baking powder, and salt.</li>
            <li>In another bowl, whisk milk, egg, melted butter, and vanilla.</li>
            <li>Combine wet and dry ingredients, stirring until smooth.</li>
            <li>Heat a pan and lightly grease with butter.</li>
            <li>Pour batter and cook until bubbles form, then flip.</li>
            <li>Cook for another 1-2 minutes, then serve warm.</li>
        </ol>

        <!-- Call-to-Action Button -->
        <button class="cta-button">Try This Recipe!</button>
    </div>
</body>
</html>


/* Import Poppins Font */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');

/* General Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  line-height: 1.6;
  color: #5a3e1b;
  background: #fff3e0; /* Light warm background */
  padding: 20px;
}

/* Container */
.container {
  max-width: 800px;
  margin: auto;
  background: #fff;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

/* Recipe Title */
#recipe-title {
  text-align: center;
  font-size: 2rem;
  color: #d2691e; /* Warm brown color */
}

/* Image Styling */
.recipe-image {
  width: 100%;
  border-radius: 10px;
  display: block;
  margin: 20px auto;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

/* Button Styling */
.cta-button {
  display: block;
  width: max-content;
  margin: 20px auto;
  padding: 10px 20px;
  background: linear-gradient(to right, #ffb347, #ffcc33); /* Pancake-inspired gradient */
  color: #5a3e1b;
  font-weight: bold;
  text-decoration: none;
  border-radius: 5px;
  transition: all 0.3s ease;
  text-align: center;
}

.cta-button:hover {
  background: linear-gradient(to right, #ffcc33, #ffb347);
  transform: scale(1.05);
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}

