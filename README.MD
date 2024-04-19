
---

1. ## Setup Node.js and npm

-   Install **_Node_** and **_npm_**
-   https://nodejs.org/en (LTS Recommended)

2. ## Initialize the MERN Starter Kit


8. ## Folder Structure

-   We are going to follow the **MVC (Model-View-Controller)** pattern for our project structure.
-   **MVC** is a _software design pattern_ that divides the application into three interconnected components: the model, the view, and the controller.
-   This pattern helps to achieve separation of concerns.
-   **Model:** Responsible for managing the data of the application. It receives user input from the controller.
-   **View:** The user interface of the application. It displays the data using the model to the user and also enables them to modify the data.
-   **Controller:** Acts as an interface between Model and View components to process all the business logic and incoming requests, manipulate data using the Model component, and interact with the Views to render the final output.

```
server/
|-- config/
|   |-- connectDB.js
|-- controllers/
|   |-- itemController.js
|-- middleware/
|   |-- asyncHandler.js
|   |-- errorHandler.js
|-- models/
|   |-- ItemModel.js
|-- routes/
|   |-- itemRouter.js
|-- .env
|-- .gitignore
|-- package.json
|-- seeder.js
|-- server.js
```
