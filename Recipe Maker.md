---
layout: page
title: Recipe Maker
search_exclude: true
permalink: /Recipe Maker/
---


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Culinary Canvas | Recipe Creator</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Poppins:wght@300;400;600&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f9f9f7;
        }
        
        .playfair {
            font-family: 'Playfair Display', serif;
        }
        
        .ingredient-item::before {
            content: "•";
            margin-right: 8px;
            color: #f59e0b;
        }
        
        .instruction-item::before {
            content: counter(step-counter);
            counter-increment: step-counter;
            margin-right: 10px;
            background-color: #f59e0b;
            color: white;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
        }
        
        .recipe-card {
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        }
        
        .recipe-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
        }
        
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
            border-radius: 10px;
        }
        
        ::-webkit-scrollbar-thumb {
            background: #d1d5db;
            border-radius: 10px;
        }
        
        ::-webkit-scrollbar-thumb:hover {
            background: #9ca3af;
        }
    </style>
</head>
<body class="min-h-screen">
    

    <main class="container mx-auto px-4 py-8">
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
            <!-- Recipe Form -->
            <div class="lg:col-span-2 bg-white rounded-xl shadow-sm p-6">
                <h2 class="playfair text-2xl font-bold text-gray-800 mb-6">Create Your Recipe Masterpiece</h2>
                
                <!-- Recipe Info -->
                <div class="mb-8">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-6">
                        <div>
                            <label for="recipe-name" class="block text-sm font-medium text-gray-700 mb-1">Recipe Name</label>
                            <input type="text" id="recipe-name" placeholder="e.g. Garlic Butter Shrimp Pasta" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-amber-500 focus:border-amber-500 transition">
                        </div>
                        <div>
                            <label for="recipe-image" class="block text-sm font-medium text-gray-700 mb-1">Image URL (optional)</label>
                            <input type="text" id="recipe-image" placeholder="https://example.com/image.jpg" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-amber-500 focus:border-amber-500 transition">
                        </div>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-6">
                        <div>
                            <label for="prep-time" class="block text-sm font-medium text-gray-700 mb-1">Prep Time (mins)</label>
                            <input type="number" id="prep-time" placeholder="15" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-amber-500 focus:border-amber-500 transition">
                        </div>
                        <div>
                            <label for="cook-time" class="block text-sm font-medium text-gray-700 mb-1">Cook Time (mins)</label>
                            <input type="number" id="cook-time" placeholder="20" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-amber-500 focus:border-amber-500 transition">
                        </div>
                        <div>
                            <label for="servings" class="block text-sm font-medium text-gray-700 mb-1">Servings</label>
                            <input type="number" id="servings" placeholder="4" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-amber-500 focus:border-amber-500 transition">
                        </div>
                    </div>
                    
                    <div>
                        <label for="recipe-description" class="block text-sm font-medium text-gray-700 mb-1">Description</label>
                        <textarea id="recipe-description" rows="3" placeholder="Describe your recipe (e.g. A creamy, garlicky shrimp pasta with fresh herbs...)" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-amber-500 focus:border-amber-500 transition"></textarea>
                    </div>
                </div>
                
                <!-- Ingredients Section -->
                <div class="mb-8">
                    <div class="flex justify-between items-center mb+4">
                        <h3 class="playfair text-xl font-bold text-gray-800">Ingredients</h3>
                        <button id="add-ingredient" class="text-amber-500 hover:text-amber-600">
                            <i class="fas fa-plus-circle text-2xl"></i>
                        </button>
                    </div>
                    <div id="ingredients-list" class="space-y-2">
                        <!-- Ingredients will be added here -->
                    </div>
                </div>
                
                <!-- Instructions Section -->
                <div class="mb-8">
                    <div class="flex justify-between items-center mb+4">
                        <h3 class="playfair text-xl font-bold text-gray-800">Instructions</h3>
                        <button id="add-instruction" class="text-amber-500 hover:text-amber-600">
                            <i class="fas fa-plus-circle text-2xl"></i>
                        </button>
                    </div>
                    <div id="instructions-list" class="space-y-4">
                        <!-- Instructions will be added here -->
                    </div>
                </div>
                
                <!-- Tags/Categories -->
                <div class="mb-8">
                    <h3 class="playfair text-xl font-bold text-gray-800 mb-4">Categories</h3>
                    <div class="flex flex-wrap gap-2">
                        <label class="inline-flex items-center">
                            <input type="checkbox" class="rounded border-gray-300 text-amber-500 focus:ring-amber-500" value="Vegetarian">
                            <span class="ml-2 text-gray-700">Vegetarian</span>
                        </label>
                        <label class="inline-flex items-center">
                            <input type="checkbox" class="rounded border-gray-300 text-amber-500 focus:ring-amber-500" value="Vegan">
                            <span class="ml-2 text-gray-700">Vegan</span>
                        </label>
                        <label class="inline-flex items-center">
                            <input type="checkbox" class="rounded border-gray-300 text-amber-500 focus:ring-amber-500" value="Gluten-Free">
                            <span class="ml-2 text-gray-700">Gluten-Free</span>
                        </label>
                        <label class="inline-flex items-center">
                            <input type="checkbox" class="rounded border-gray-300 text-amber-500 focus:ring-amber-500" value="Dairy-Free">
                            <span class="ml-2 text-gray-700">Dairy-Free</span>
                        </label>
                        <label class="inline-flex items-center">
                            <input type="checkbox" class="rounded border-gray-300 text-amber-500 focus:ring-amber-500" value="Quick-Meal">
                            <span class="ml-2 text-gray-700">Quick Meal</span>
                        </label>
                    </div>
                </div>
                
                <div class="flex justify-end">
                    <button id="generate-recipe" class="bg-amber-500 hover:bg-amber-600 text-white px-6 py-3 rounded-full font-medium transition flex items-center space-x-2">
                        <i class="fas fa-magic"></i>
                        <span>Generate Recipe Card</span>
                    </button>
                </div>
            </div>
            
            <!-- Recipe Preview -->
            <div class="lg:sticky lg:top-8 lg:h-fit">
                <div id="recipe-preview" class="bg-white rounded-xl shadow-sm p-6">
                    <div class="text-center py-12">
                        <i class="fas fa-utensils text-5xl text-gray-300 mb-4"></i>
                        <h3 class="playfair text-xl font-bold text-gray-600">Your recipe will appear here</h3>
                        <p class="text-gray-500">Fill out the form to see a preview</p>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <footer class="bg-gray-50 mt-16 py-8">
        <div class="container mx-auto px-4 text-center text-gray-500">
            <p>© 2023 Culinary Canvas. All recipes created are property of their creators.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Counter for ingredients and instructions
            let ingredientCount = 0;
            let instructionCount = 0;
            
            // Add ingredient field
            document.getElementById('add-ingredient').addEventListener('click', function() {
                ingredientCount++;
                const ingredientDiv = document.createElement('div');
                ingredientDiv.className = 'flex items-start space-x-2';
                ingredientDiv.innerHTML = `
                    <input type="text" placeholder="1 cup flour" class="flex-1 px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-amber-500 focus:border-amber-500 transition ingredient-input">
                    <button class="text-red-400 hover:text-red-600 remove-ingredient" type="button">
                        <i class="fas fa-times"></i>
                    </button>
                `;
                document.getElementById('ingredients-list').appendChild(ingredientDiv);
            });
            
            // Remove ingredient field
            document.getElementById('ingredients-list').addEventListener('click', function(e) {
                if (e.target.closest('.remove-ingredient')) {
                    e.target.closest('.flex').remove();
                }
            });
            
            // Add instruction field
            document.getElementById('add-instruction').addEventListener('click', function() {
                instructionCount++;
                const instructionDiv = document.createElement('div');
                instructionDiv.className = 'flex items-start space-x-2';
                instructionDiv.innerHTML = `
                    <textarea placeholder="Step ${instructionCount}..." rows="2" class="flex-1 px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-amber-500 focus:border-amber-500 transition instruction-input"></textarea>
                    <button class="text-red-400 hover:text-red-600 remove-instruction mt-2" type="button">
                        <i class="fas fa-times"></i>
                    </button>
                `;
                document.getElementById('instructions-list').appendChild(instructionDiv);
            });
            
            // Remove instruction field
            document.getElementById('instructions-list').addEventListener('click', function(e) {
                if (e.target.closest('.remove-instruction')) {
                    e.target.closest('.flex').remove();
                }
            });
            
            // Generate recipe preview
            document.getElementById('generate-recipe').addEventListener('click', function() {
                const recipeName = document.getElementById('recipe-name').value || 'Untitled Recipe';
                const recipeImage = document.getElementById('recipe-image').value;
                const prepTime = document.getElementById('prep-time').value || 'N/A';
                const cookTime = document.getElementById('cook-time').value || 'N/A';
                const servings = document.getElementById('servings').value || 'N/A';
                const description = document.getElementById('recipe-description').value || 'No description provided.';
                
                // Get ingredients
                const ingredientInputs = document.querySelectorAll('.ingredient-input');
                const ingredients = [];
                ingredientInputs.forEach(input => {
                    if (input.value.trim()) ingredients.push(input.value);
                });
                
                // Get instructions
                const instructionInputs = document.querySelectorAll('.instruction-input');
                const instructions = [];
                instructionInputs.forEach((input, index) => {
                    if (input.value.trim()) instructions.push(input.value);
                });
                
                // Get selected categories
                const checkboxes = document.querySelectorAll('input[type="checkbox"]:checked');
                const categories = [];
                checkboxes.forEach(checkbox => {
                    categories.push(checkbox.value);
                });
                
                // Generate the preview HTML
                let previewHTML = `
                    <div class="recipe-card">
                        ${recipeImage ? `<img src="${recipeImage}" alt="${recipeName}" class="w-full h-64 object-cover rounded-t-xl mb-4">` : ''}
                        <h2 class="playfair text-3xl font-bold text-gray-800 mb-2">${recipeName}</h2>
                        
                        <div class="flex items-center space-x-4 text-gray-600 mb-4">
                            ${prepTime !== 'N/A' ? `<div class="flex items-center space-x-1">
                                <i class="fas fa-clock"></i>
                                <span>Prep: ${prepTime} min</span>
                            </div>` : ''}
                            
                            ${cookTime !== 'N/A' ? `<div class="flex items-center space-x-1">
                                <i class="fas fa-fire"></i>
                                <span>Cook: ${cookTime} min</span>
                            </div>` : ''}
                            
                            ${servings !== 'N/A' ? `<div class="flex items-center space-x-1">
                                <i class="fas fa-utensils"></i>
                                <span>${servings} servings</span>
                            </div>` : ''}
                        </div>
                        
                        ${description ? `<p class="text-gray-700 mb-6">${description}</p>` : ''}
                        
                        ${categories.length > 0 ? `
                        <div class="flex flex-wrap gap-2 mb-6">
                            ${categories.map(cat => `<span class="bg-amber-100 text-amber-800 text-xs px-3 py-1 rounded-full">${cat}</span>`).join('')}
                        </div>` : ''}
                        
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-8">
                            <div>
                                <h3 class="playfair text-xl font-bold text-gray-800 mb-4 border-b pb-2">Ingredients</h3>
                                <ul class="space-y-2">
                                    ${ingredients.length > 0 ? 
                                        ingredients.map(ing => `<li class="ingredient-item text-gray-700">${ing}</li>`).join('') :
                                        '<li class="text-gray-500">No ingredients added</li>'
                                    }
                                </ul>
                            </div>
                            
                            <div>
                                <h3 class="playfair text-xl font-bold text-gray-800 mb-4 border-b pb-2">Instructions</h3>
                                <ol class="list-decimal list-inside space-y-3" style="counter-reset: step-counter;">
                                    ${instructions.length > 0 ? 
                                        instructions.map((inst, idx) => 
                                            `<li class="instruction-item text-gray-700 ml-6 pl-2">${inst}</li>`
                                        ).join('') :
                                        '<li class="text-gray-500">No instructions added</li>'
                                    }
                                </ol>
                            </div>
                        </div>
                        
                        <div class="border-t pt-4 text-center text-gray-500">
                            <p>Recipe created with <span class="text-amber-500">Culinary Canvas</span></p>
                        </div>
                    </div>
                `;
                
                document.getElementById('recipe-preview').innerHTML = previewHTML;
                document.getElementById('print-btn').classList.remove('hidden');
            });
            
            // Print functionality
            document.getElementById('print-btn').addEventListener('click', function() {
                const printContent = document.getElementById('recipe-preview').innerHTML;
                const originalContent = document.body.innerHTML;
                
                document.body.innerHTML = `
                    <div class="container mx-auto p-8 max-w-3xl">
                        ${printContent}
                    </div>
                `;
                
                window.print();
                document.body.innerHTML = originalContent;
                window.location.reload();
            });
            
            // Add initial ingredient and instruction fields
            document.getElementById('add-ingredient').click();
            document.getElementById('add-instruction').click();
        });
    </script>
</body>
</html>