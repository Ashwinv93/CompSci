---
toc: true
comments: false
layout: post
title: Recipie Finder
type: tangibles
courses: { compsci: {week: 3} }
---

<html>
<head>
    <title>Recipe Finder</title>
</head>
<body>
    <h1>Recipe Finder</h1>
    <p>Enter a list of ingredients separated by commas:</p>
    <input type="text" id="ingredientInput">
    <button id="searchButton">Search</button>
    <h2>Recipes:</h2>
    <ul id="recipeList"></ul>
    <script>
        const apiKey = 'a47087a81974fac6c875124c22f5b99b'; // Replace with your Edamam API key
        document.getElementById('searchButton').addEventListener('click', searchRecipes);
        function searchRecipes() {
            const ingredientInput = document.getElementById('ingredientInput').value;
            const recipeList = document.getElementById('recipeList');
            // Clear previous results
            recipeList.innerHTML = '';
            // Make a request to the Edamam API
            fetch(`https://api.edamam.com/search?q=${ingredientInput}&app_id=YOUR_APP_ID&app_key=${apiKey}`)
                .then(response => response.json())
                .then(data => {
                    const recipes = data.hits;
                    recipes.forEach(recipe => {
                        const recipeTitle = recipe.recipe.label;
                        const recipeURL = recipe.recipe.url;
                        // Create list items with recipe titles and links
                        const listItem = document.createElement('li');
                        const link = document.createElement('a');
                        link.href = recipeURL;
                        link.textContent = recipeTitle;
                        listItem.appendChild(link);
                        recipeList.appendChild(listItem);
                    });
                })
                .catch(error => {
                    console.error('Error fetching recipes:', error);
                });
        }
    </script>
</body>
</html>