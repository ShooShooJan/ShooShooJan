<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Veggie and Herb Mac and Cheese Recipe</title>
  <style>
    /* Basic Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: Arial, sans-serif;
      color: #333;
      background-color: #fdf5e6;
    }
    /* Layout Styles */
    .container {
      max-width: 900px;
      margin: 0 auto;
      padding: 20px;
    }
    header {
      text-align: center;
      padding: 20px;
    }
    header h1 {
      color: #4b5320;
    }
    header p {
      color: #666;
      font-size: 1.1em;
    }
    /* Ingredients and Instructions */
    .recipe-section {
      display: flex;
      justify-content: space-between;
      gap: 20px;
      margin-top: 20px;
    }
    .ingredients, .instructions {
      flex: 1;
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
    .ingredients h2, .instructions h2 {
      color: #4b5320;
      margin-bottom: 10px;
    }
    .ingredients ul, .instructions ol {
      list-style-type: none;
    }
    /* Optional Tooltip for Ingredient Hints */
    .ingredient-item:hover::after {
      content: "This ingredient brings a unique flavor!";
      position: absolute;
      background-color: #fffae5;
      padding: 5px;
      font-size: 0.8em;
      border-radius: 4px;
      color: #555;
      margin-left: 5px;
    }
    /* Collapsible Nutrition Panel */
    .collapsible {
      cursor: pointer;
      padding: 10px;
      border: none;
      text-align: left;
      outline: none;
      font-size: 1.1em;
      background-color: #4b5320;
      color: white;
      border-radius: 8px;
      margin-top: 20px;
    }
    .content {
      padding: 0 20px;
      display: none;
      overflow: hidden;
      background-color: #fff;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      border-radius: 8px;
      margin-top: 5px;
    }
    /* Comments and Rating */
    .comments {
      margin-top: 30px;
    }
    .comments h2 {
      color: #4b5320;
    }
    .rating {
      display: flex;
      gap: 5px;
    }
    .star {
      color: gold;
      font-size: 1.5em;
    }
  </style>
</head>
<body>

<div class="container">
  <!-- Header -->
  <header>
    <h1>Veggie and Herb Mac and Cheese</h1>
    <p>A creamy, veggie-packed twist on classic comfort food, perfect for any night.</p>
    <img src="path/to/mac_and_cheese_image.jpg" alt="Mac and Cheese with Veggies and Herbs" style="width:100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);">
  </header>

  <!-- Recipe Section -->
  <div class="recipe-section">
    <!-- Ingredients -->
    <div class="ingredients">
      <h2>Ingredients</h2>
      <ul>
        <li class="ingredient-item">8 oz elbow macaroni</li>
        <li class="ingredient-item">2 tbsp butter</li>
        <li class="ingredient-item">2 cloves garlic, minced</li>
        <li class="ingredient-item">1 small onion, finely chopped</li>
        <li class="ingredient-item">1 small zucchini, diced</li>
        <li class="ingredient-item">1 small bell pepper, diced</li>
        <li class="ingredient-item">1 cup broccoli florets, chopped</li>
        <li class="ingredient-item">1 cup baby spinach (optional)</li>
        <li class="ingredient-item">2 cups milk</li>
        <li class="ingredient-item">1 cup shredded cheddar cheese</li>
        <li class="ingredient-item">1/4 cup Parmesan cheese</li>
        <li class="ingredient-item">Fresh parsley, basil, thyme</li>
      </ul>
    </div>

    <!-- Instructions -->
    <div class="instructions">
      <h2>Instructions</h2>
      <ol>
        <li>Cook the pasta until al dente. Drain and set aside.</li>
        <li>Sauté the garlic, onion, zucchini, bell pepper, and broccoli in butter until tender.</li>
        <li>Stir in spinach until wilted.</li>
        <li>In the same skillet, make the cheese sauce by stirring in flour and milk, then add cheeses.</li>
        <li>Add herbs and combine with pasta and veggies. Serve warm.</li>
      </ol>
    </div>
  </div>

  <!-- Collapsible Nutrition Information -->
  <button type="button" class="collapsible">Nutrition Information</button>
  <div class="content">
    <p>Calories: 450 per serving | Protein: 18g | Carbs: 56g | Fat: 18g</p>
  </div>

  <!-- Comments and Rating Section -->
  <div class="comments">
    <h2>Comments</h2>
    <p>What did you think of the recipe? Leave your rating:</p>
    <div class="rating">
      <span class="star">★</span>
      <span class="star">★</span>
      <span class="star">★</span>
      <span class="star">★</span>
      <span class="star">★</span>
    </div>
  </div>
</div>

<script>
  // Collapsible Nutrition Info
  document.querySelectorAll('.collapsible').forEach(button => {
    button.addEventListener('click', function () {
      this.classList.toggle('active');
      let content = this.nextElementSibling;
      content.style.display = content.style.display === 'block' ? 'none' : 'block';
    });
  });
</script>

</body>
</html>
