# The Project Description
The AI-Powered Menu Search is a web application built with Node.js and Express.js that allows users to upload an image of a restaurant menu. The application then uses the OpenAI API to analyze the menu and search for specific dishes (in this case, tartare, pizza, and spaghetti). The results are presented to the user in a clean, easy-to-read format.

Key features of the project include:

* File upload functionality for menu images
* Integration with OpenAI API for image analysis
* User-friendly interface built with Bootstrap
* Dockerized application for easy deployment and scaling

This project serves as a proof of concept, demonstrating how AI can be used to extract meaningful information from images in a way that's more flexible and potentially more powerful than traditional web scraping methods.

## How to Run
To run this project, follow these steps:

1. Clone the repository from GitHub
2. Ensure you have Docker installed on your system
3. Navigate to the project directory in your terminal
4. Create a `.env` file with the following settings:

```
ORGANIZATION=your_openai_organization
PROJECT=your_openai_project
API_KEY=your_openai_api_key
```

This ensures that sensitive data like the API key is not exposed in the codebase.

5. Build the Docker image:

```
docker build -t find_dish_site .
```

6. Run the Docker container:

```
docker run -p 3000:3000 find_dish_site
```

7. Open your web browser and go to http://localhost:3000

You should now see the application running and be able to upload menu images for analysis.

## Link to the Post
For more detailed information about the development process and technical details, you can read the full blog post at: [Create an AI-Powered Menu Search with Node.js and Express.js](https://blog.hsh303.pl/posts/code/create-an-ai-powered-menu-search-with-node.js-and-express.js/)
