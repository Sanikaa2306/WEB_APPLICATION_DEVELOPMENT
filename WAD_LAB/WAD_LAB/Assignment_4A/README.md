Step-by-Step Procedure:

1. Create Project Folder Structure
   jquery-mobile-site/
   │
   ├── index.html
   └── (All content can be inside this single HTML file)

2. Include jQuery Mobile CDN Links in index.html
   <!DOCTYPE html>
   <html>
   <head>
   <title>Simple Mobile Website</title>
   <!-- Meta tag for responsive design -->
   <meta name="viewport" content="width=device-width, initial-scale=1">

   <!-- jQuery and jQuery Mobile CSS/JS CDN -->
   <link rel="stylesheet" href="https://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css">
   <script src="https://code.jquery.com/jquery-1.11.3.min.js"></script>
   <script src="https://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script>
   </head>
   <body>

   <!-- Page 1 -->
   <div data-role="page" id="home">
       <div data-role="header">
       <h1>Welcome</h1>
       </div>
       <div data-role="content">
       <p>This is a simple mobile website using jQuery Mobile.</p>
       <a href="#about" data-role="button">Go to About Page</a>
       </div>
       <div data-role="footer">
       <h4>Home Page Footer</h4>
       </div>
   </div>

   <!-- Page 2 -->
   <div data-role="page" id="about">
       <div data-role="header">
       <h1>About</h1>
       </div>
       <div data-role="content">
       <p>This page gives information about the website.</p>
       <a href="#home" data-role="button">Back to Home</a>
       </div>
       <div data-role="footer">
       <h4>About Page Footer</h4>
       </div>
   </div>

   </body>
   </html>

3. Open the Website in a Browser
   run a live server.
   The website will automatically adjust for mobile screens.
