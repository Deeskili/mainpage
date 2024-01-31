---
toc: false
comments: false
layout: post
title: First Iteration Test
description: Does Not Work 
type: hacks
courses: { compsci: {week: 8} }
---


<html>
<head>
    <title>Recipe Input</title>
</head>
<body>
    <h1>Enter Recipe</h1>
    <form>
        <label for="recipeName">Recipe Title:</label>
        <input type="text" id="recipeName" name="recipeName"><br>

        <label for="recipeText">Recipe:</label>
        <textarea id="recipeText" name="recipeText" rows="10" cols="40"></textarea><br>

        <button onclick="submitRecipe()">Submit Recipe</button>
    </form>

    <script>
        function submitRecipe() {
            const recipeName = document.getElementById("recipeName").value;
            const recipeText = document.getElementById("recipeText").value;

            if (recipeName && recipeText) {
                // Send the data to the backend for storage
                fetch('/api/editedrecipe/addrecipe', {
                    method: 'POST',
                    headers: {
                        'Content-Type': 'application/json'
                    },
                    body: JSON.stringify({
                        title: recipeName,
                        ingredients: recipeText,
                        instructions: '',
                        image_name: '',
                        cleaned_ingredients: '',
                        edited_by: 'User'
                    })
                })
                .then(response => response.json())
                .then(data => {
                    alert(data.message);
                })
                .catch(error => console.error('Error submitting recipe:', error));
            } else {
                alert('Please fill in both the title and the recipe text.');
            }
        }
    </script>
</body>
</html>
