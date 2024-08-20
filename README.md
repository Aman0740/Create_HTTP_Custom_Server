# Create_HTTP_Custom_Server


1. **Setup the Project:**
   - **Create a Directory:** You start by creating a new directory for your project and navigating into it.
   - **Initialize Node.js Project:** By running `npm init -y`, you initialize a new Node.js project which creates a `package.json` file. This file keeps track of your project's dependencies and scripts.
   - **Install Express.js:** You install Express.js, a popular web framework for Node.js, which helps in handling HTTP requests and routing more easily.

2. **Create and Configure the Server:**
   - **Create `db.json`:** You create a `db.json` file containing some sample data. This file will be used to simulate a database, providing product and user information.
   - **Write the Server Code:** In the `server.js` file:
     - **Import Modules:** You import the required modules: Express for setting up the server, and `fs` and `path` for reading from the `db.json` file.
     - **Initialize Express:** You create an Express application instance.
     - **Set Up Middleware:** You add middleware to parse JSON bodies, which allows your server to handle incoming JSON data.
     - **Define Routes:** You define different routes (or endpoints) for the server:
       - `/home`: Responds with a welcome message.
       - `/about`: Responds with an about message.
       - `/getproductdata`: Reads data from `db.json` and returns the product information.
       - `/user`: Reads data from `db.json` and returns the user information.
     - **Start the Server:** Finally, you set the server to listen on port 3000 and log a message indicating that it’s running.

3. **Run the Server:**
   - **Add a Start Script:** You add a script in the `package.json` file to simplify starting the server.
   - **Start the Server:** By running `npm start`, the server starts up, listens for incoming requests, and responds according to the defined routes.

4. **Access the Endpoints:**
   - You can now open a web browser or a tool like Thunder Client (or Postman) and visit the endpoints to see how the server responds:
     - **`/home`** and **`/about`** return simple text messages.
     - **`/getproductdata`** and **`/user`** return data read from the `db.json` file in JSON format.
