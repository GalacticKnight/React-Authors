Step 1 (set up the Back-End):
mkdir <project>
cd <project>
mkdir server
cd server
touch server.js

""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""Add this to you server.js you created
const port = 8000;
const express = require('express');
const app = express();

app.use(express.json(), express.urlencoded({ extended: true }));

// CORS FOR FRONT END 
// const cors = require("cors");
// app.use(cors({ //cors is going to allow different ports to send requests to our API
//     origin:"http://localhost:3000" 
// }));

// ROUTES AND CONFIG AFTER MAKING FILES
// require("./config/mongoose.config");
// const xRoutes = require("./routes/xxxx");
// xRoutes(app);

app.listen(port, () => console.log(`🎉Party on port: ${port}`) );
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

mkdir controllers routes models config
npm install express mongoose cors bcrypt dotenv jsonwebtoken
npm i -g nodemon


Step 2(Set up the Front-End):
npx create-react-app client
cd client
npm install axios react-router-dom


Step 1-2(After you set everything, these are the terminal commands to start them):
npm start
nodemon server.js








