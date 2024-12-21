# CRAFT & COOK

#### Description:

# Craft and Cook Development Process  

**Craft and Cook** is a web app designed to help users discover recipes based on the ingredients they already have. This project was my final submission for CS50, combining everything I’ve learned throughout the course into a practical, creative application. Below, I’ll share the journey of building this app, from concept to deployment, along with the challenges and lessons learned.  

---

## Concept and Planning  

The idea for Craft and Cook stemmed from a common frustration many people experience: deciding what to cook without having to buy additional ingredients. Too often, ingredients sit unused in pantries or refrigerators, eventually going to waste. I wanted to create a solution that not only minimizes food waste but also inspires creativity in the kitchen.  

The app’s purpose was clear:  
- Allow users to input ingredients they already have.  
- Fetch recipe suggestions tailored to those ingredients.  
- Present a simple, intuitive interface that anyone can navigate easily.  

To achieve this, I researched recipe APIs and discovered the [Spoonacular API](https://spoonacular.com/food-api). This API stood out because of its extensive recipe database and advanced filtering capabilities, making it ideal for ingredient-based queries.  

I began sketching the app’s design, identifying the main features, and outlining a plan for development. The project was broken down into three phases: backend development, frontend design, and deployment.  

---

## Building the App  

### Backend Development  
The backend was built using Python, which I selected for its simplicity and robust libraries. Python provided a straightforward way to handle user inputs and communicate with the Spoonacular API.  

The development process began with creating functions to accept ingredient inputs from users. These inputs were then formatted into a query string, which was sent to the API. The API’s response contained various recipe details, such as titles, images, and links to instructions.  

I also included error handling in the backend to ensure the app could manage issues like invalid inputs, empty fields, or API downtime. For example, if a user left the input field blank or entered gibberish, the app would display an error message prompting them to try again.  

### Frontend Design  
The frontend was built using HTML and CSS, focusing on creating a clean and responsive design. I wanted the app to be accessible on both desktop and mobile devices, ensuring users could search for recipes conveniently, whether in their kitchens or on the go.  

The main page features:  
- A text input field for entering ingredients.  
- A "Find Recipes" button to submit the query.  
- A results section displaying recipe titles, images, and links to detailed instructions.  

I opted for a minimalist aesthetic to keep the focus on functionality. A simple color scheme and intuitive layout make the app welcoming for users of all tech skill levels.  

### API Integration  
The integration of the Spoonacular API was a critical component of the app. By sending user inputs to the API and processing its JSON responses, I could provide dynamic recipe suggestions. This involved writing functions to parse the API’s data and display it meaningfully.  

---

## Testing  

Testing was an ongoing process throughout development. I tested the app with various ingredient combinations to ensure it returned accurate and relevant recipes. Common scenarios included:  
- Entering single ingredients, such as “tomato” or “chicken.”  
- Combining multiple ingredients to see how well the API handled complex queries.  
- Testing invalid inputs, like leaving the field empty or entering nonsensical words.  

I also checked the app’s responsiveness by using it on different devices, ensuring the layout adjusted properly on smaller screens.  

Through this testing process, I identified and resolved issues like:  
- Ensuring results were sorted by relevance.  
- Preventing errors when the API returned no recipes.  

---

## Deployment  

With the app fully functional, I turned to deployment. For this, I chose **Vercel**, a platform known for its simplicity and speed. Vercel allowed me to connect my GitHub repository for seamless deployment and manage environment variables, such as my API key, securely.  

Deployment steps included:  
1. Uploading my code to GitHub.  
2. Configuring Vercel to deploy the app automatically upon updates.  
3. Testing the live app to ensure it performed as expected in a production environment.  

The final result was an app accessible globally, allowing anyone with an internet connection to use Craft and Cook.  

---

## Challenges  

Building Craft and Cook came with its fair share of challenges:  
1. **API Limitations**: Spoonacular’s rate limits required careful planning to avoid exceeding the number of allowed requests.  
2. **Error Handling**: Ensuring the app provided meaningful feedback when the user input was invalid or when the API failed.  
3. **Responsive Design**: Adjusting the layout to look good on both large screens and smaller mobile devices took extra effort.  

Each challenge offered valuable learning opportunities, helping me improve my problem-solving and debugging skills.  

---

## Lessons Learned  

This project was an invaluable learning experience that taught me:  
- **Working with APIs**: I gained hands-on experience fetching and processing data from an external source.  
- **Building User Interfaces**: Creating a responsive design reinforced the importance of user-friendly layouts.  
- **Iterative Development**: Continuously testing and refining the app led to a more polished final product.  
- **Deployment Best Practices**: I learned how to secure sensitive data, like API keys, during deployment.  

---

## Future Plans  

Craft and Cook has significant potential for growth. Here are some features I plan to add in the future:  
- **User Accounts**: Allow users to save their favorite recipes and access them later.  
- **Meal Planning**: Introduce a feature for weekly meal planning based on the user’s inventory.  
- **Dietary Preferences**: Add filters for vegan, vegetarian, or gluten-free recipes.  

---

## Conclusion  

Developing Craft and Cook has been one of the most rewarding experiences of my journey into computer science. It brought together everything I’ve learned in CS50, from Python programming to web development and deployment.  

This app reflects not just technical skills but also creativity and problem-solving. It’s a project I’m proud to share, and I hope it inspires others to explore the endless possibilities of coding.  

Thank you for reading, and happy cooking!
