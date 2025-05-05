## For given project :

1. Go to tha path : static-website/

2. Install all packages
   npm install / npm i

3. Run the Server
   node server.js
   Open your browser and navigate to:
   http://localhost:3000

-------------xxxxxxxxxx--------------

## For new project:

Step-by-Step Procedure:

1. Initialize a Node.js Project
   mkdir static-website
   cd static-website
   npm init -y

2. Install Express.js
   npm install express

3. Create Project Structure
   static-website/
   │
   ├── public/
   │ ├── index.html
   │ ├── style.css
   │ └── script.js
   │
   └── server.js

4. Create index.html in the public Folder
   <!-- public/index.html -->
   <!DOCTYPE html>
   <html>
   <head>
     <title>My Static Website</title>
     <link rel="stylesheet" href="style.css">
   </head>
   <body>
     <h1>Welcome to My Static Website</h1>
     <p>This site is served using Node.js and Express.</p>
     <script src="script.js"></script>
   </body>
   </html>

5. Create style.css
   <!-- public/style.css -->

   body {
   font-family: Arial, sans-serif;
   text-align: center;
   background-color: #f0f0f0;
   }

6. Create script.js
   <!-- public/script.js -->

   console.log("Static site loaded successfully!");

7. Create server.js File
   <!-- server.js -->

   const express = require('express');
   const app = express();
   const port = 3000;

   // Serve static files from the 'public' directory
   app.use(express.static('public'));

   // Start the server
   app.listen(port, () => {
   console.log(`Server is running at http://localhost:${port}`);
   });

8. Run the Server
   node server.js
   Open your browser and navigate to:
   http://localhost:3000
