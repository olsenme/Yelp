# Airbnb-Like-API

# Instructions

1. Clone Repo ``` git clone https://github.com/olsenme/AirbnbAPI.git```
2. Install dependencies ```npm install```
3. Start up the API ```docker-compose up api```
4. Start up mySql and Mongo DB ```docker-compose up mongo mysql```
5. Send appropriate queries (using cURL, Postman, etc.) to ```http://localhost:3000/```

# Dicussion
I used NodeJS,mySql,mongoDB,Docker,and JWT to build this API.

# Requirements

<b>Design and build a RESTFUL API for a Yelp-like application. <b> <br>
  <ul>
    <li>The application will be centered around businesses and user reviews of businesses in US cities. </li>
    <li>Users may add their business to the application.</li>
    <li> Business information shall include:
        <ul>
          <li>Business name </li>
          <li>Business street name</li>
          <li>Business city</li>
          <li>Business state</li>
          <li>Business ZIP code</li>
          <li>Business phone number</li>
          <li>Business categories and subcategories</li>
          <li>Business website(optional)</li>
          <li>Business email(optional)</li>
      </ul>
     </li>
    <li>Users may register with a username and password.</li>
    <li>Users may modify any of the information listed above for an already-existing business they own.</li>
    <li>Users may remove a business from the application.</li>
    <li>Users may get a list of businesses.</li>
    <li>Users may fetch detailed information about a business.</li>
    <li>Detailed business information will include all of the information described above as well as reviews of the business and photos of the business.</li>
    <li>Users may write a review of an existing business. </li>
    <li>Business information shall include:</li>
     <ul>
       <li>A "star" rating between 0 and 5 (e.g. 4 stars) </li>
       <li>A "dollar sign" rating between 1 and 4, indicating how expensive the business is (e.g. 2 dollar signs)</li>
       <li>A written review(optional)</li>
    </ul>
    <li>A user may write at most one review of any business.</li>
    <li>Users may modify or delete any review they've written.</li>
    <li>Users may upload image files containing photos of an existing business. </li>
    <li> Each photo may have an associated caption(optional).</li>
    <li>Users may remove any photo they've uploaded, and they may modify the caption of any photo they've uploaded.</li>
    <li>Users may list all of the businesses they own.</li>
    <li>Users may list all of the reviews they've written.</li>
    <li>Users may list all of the photos they've uploaded.</li>
    <li>Users may create categories and subcategories that will be used when creating businesses.</li>
    <li>Categories and subcategories are the following:</li>
    <ul>
       <li>Restaurant </li>
        <ul>
          <li>Pizza</li>
          <li>Mexican</li>
          <li>Chinese</li>
          <li>Brewpub</li>
      </ul>
       <li>Shopping </li>
      <ul>
          <li>Grocery store</li>
          <li>Flowers</li>
          <li>Clothing</li>
          <li>Hardware</li>
      </ul>
      <li>Arts and Entertainment </li>
      <ul>
          <li>Museum</li>
          <li>Art gallery</li>
          <li>Movie theater</li>
      </ul>
    </ul>
      <li>Users may delete or modify categories and subcategories.</li>
      <li>Users may list all categories. </li>
      <li>Users may list all subcategories associated with a given category.</li>
      <li>Registered users may log in with their username and password.</li><br>
    
<b>Implement endpoints<b><br>
  
  <li>Port will be 8003.</li>
  <li>Endpoints will have paginated responses where appropriate. </li>
  <li>Each API endpoint will respond with an appropriate HTTP status code and, when needed, a response body.</li>
  <li>Any API endpoint that takes a request body will perform basic verification of the data provided in the request body.</li>
  <li>Any API endpoint with a parameterized route will perform basic verification of the specified route parameters.</li>
  <li>A route will be included to implement each of the API endpoints in design. </li>
  <li>Server will be containerized into a Docker image with runtime dependencies.</li>
  <p>Containers launched from this image will automatically start the server listening on a specified port, and one should be able to successfully make requests to the containerized server from the outside world (e.g. from your host machine).</p>
<li><b>A MySQL database will be used to store:<b></li>
  <ul>
    <li>Businesses</li>
    <li>Reviews</li>
    <li>Photos</li>
  </ul>
  <li>Official MYSQL Docker Image will be used to power MySQL database.</li>
  <li>Database script will be used to initialize MySQL database upond first launch of container.</li>
  <li>Database will be persisted in Docker voume.</li>
   <li>API server will read the location(hostname,database Name) and credentials(username and password) from environment variables.</li><br>
  <b>A MongoDB will be used to store:<b>
    <ul>
      <li>Username</li>
      <li>Email Address</li>
      <li>Hashed/salted password</li>
    </ul>
    <li>Official Mongo Docker Image will be used to power MySQL database.</li>
    <li>Script will be written to create a low-privileged user to use to connect to MongoDB server from Node.js.</li>
    <li>Three container application will be created and run via Docker Compose. </li>
  </ul>
    
  
  
  
  
  
  
  
  
  

