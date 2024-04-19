<img src="./MERN.png">

### This template provides a minimal MERN setup. It's configured to use `pnpm` as the package manager.

1. ## Setup Node.js, npm, pnpm and degit

-   Install **_Node_** and **_npm_**

    -   Download the latest version of Node.js and npm from [here](https://nodejs.org/en).
    -   Install Node.js and npm by following the installation wizard.

-   Install **_pnpm_** globally by running the following command in your terminal:

```bash
npm install -g pnpm
```

-   Install **_degit_** globally by running the following command in your terminal:

```bash
npm install -g degit
```

2. ## Initialize the MERN Starter Kit

### Option 1: Clone the Repository and Remove Git History

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/Pilag6/MERN.git
    ```

2. **Navigate to the Project Directory:**

    ```bash
    cd MERN
    ```

3. **Remove Existing Git History:**

    ```bash
    rm -rf .git
    ```

    This command will remove the existing Git history. That way, you can start fresh with your own Git repository.

4. **Initialize a New Git Repository:**

    ```bash
    git init
    ```

    This command initializes a new Git repository for your project.

5. **Install Dependencies using pnpm:**

    ```bash
    cd client
    pnpm install

     cd ../server
     pnpm install
    ```

    This command installs project dependencies using pnpm. If you don't have pnpm installed, you can install it globally using `npm install -g pnpm`.

6. **Run the Development Server and Client :**

    ```bash
    cd client
    pnpm run dev

    cd ../server
    pnpm run dev
    ```

    This command will start the development server in the port `http://localhost:3300`, and you can access your React application at `http://localhost:5173`.

### Option 2: Use degit

Alternatively, you can use `degit` to scaffold the template without cloning the entire repository.

1. **Use degit to Fetch the Template:**

    ```bash
    npx degit Pilag6/MERN my-MERN-app
    ```

    This command fetches the template without Git history and renames the project to `my-MERN-app`. You can replace `my-MERN-app` with your preferred project name.

    If you don't have `degit` installed, you can install it globally using `npm install -g degit`.

2. **Navigate to the Project Directory:**

    ```bash
    cd my-MERN-app
    ```

3. **Initialize a New Git Repository:**

    ```bash
    git init
    ```

    This command initializes a new Git repository for your project.

4. **Install Dependencies using pnpm:**

    ```bash
    cd client
    pnpm install

    cd ../server
    pnpm install
    ```

    This command installs project dependencies using pnpm. If you don't have pnpm installed, you can install it globally using `npm install -g pnpm`.

5. **Run the Development Server:**

    ```bash
    cd client
    pnpm run dev

    cd ../server
    pnpm run dev
    ```

    This command will start the development server in the port `http://localhost:3300`, and you can access your React application at `http://localhost:5173`.

6. ## Folder Structure

-   We are going to follow the **MVC (Model-View-Controller)** pattern for our project structure.
-   **MVC** is a _software design pattern_ that divides the application into three interconnected components: the model, the view, and the controller.
-   This pattern helps to achieve separation of concerns.
-   **Model:** Responsible for managing the data of the application. It receives user input from the controller.
-   **View:** The user interface of the application. It displays the data using the model to the user and also enables them to modify the data.
-   **Controller:** Acts as an interface between Model and View components to process all the business logic and incoming requests, manipulate data using the Model component, and interact with the Views to render the final output.

```
client/
|-- serc/
|   |-- connectDB.js
|   |-- asyncHandler.js
|-- controllers/
|   |-- Controller.js
|   |-- AuthController.js
|-- middleware/
|   |-- errorHandler.js
|-- models/
|   |-- Model.js
|   |-- userModel.js
|-- routes/
|   |-- Router.js
|   |-- AuthRouter.js
|-- .eslintrccjs
|-- .gitignore
|-- index.html
|-- jsconfig.json
|-- package.json
|-- vite.config.js

server/
|-- config/
|   |-- connectDB.js
|   |-- asyncHandler.js
|-- controllers/
|   |-- Controller.js
|   |-- AuthController.js
|-- middleware/
|   |-- errorHandler.js
|-- models/
|   |-- Model.js
|   |-- userModel.js
|-- routes/
|   |-- Router.js
|   |-- AuthRouter.js
|-- .env
|-- .gitignore
|-- package.json
|-- seeder.js
|-- server.js
```
