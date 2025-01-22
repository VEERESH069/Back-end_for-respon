# Back-end_for-respon
Response 
4
5
6
7
1
For Legend
22/1/2025
Making your 1st api poge.
S1.Create repo in git, create readmd there.
S2. Clone it to vs code.
S3. npm init -y
npm i express dotenv
create file index.js
create file name (.env)
The below we should write in the index.js{
const express = require (“express”);
const app = express();
const port = 3000;
app.get(‘/assistant/greet’ ,(req,res)=>{
// go to thunder client (in Get, method (https://localhost:3000/assistant/greet)
// in parameter(write name in query)
const name = req.query.name; =>// if u write in json format we should write as 
(req.json.name);
const date = new Date().getDay();
const dayMessage = [ // greetings that given by kalvium in assignment]
res.send ({
“WelcomeMessage” : `hello, ${name}! Welcome to our assistant app!”
“dayMessage” : dayMessage[date]
})
app.listen(port,()=>{
 console.log(`Server is running in port ${port}`)
})
After writing the code run the server by the below command{ 
node —watch index.js
