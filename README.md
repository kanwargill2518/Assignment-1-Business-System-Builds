# Codin 1 Website Docker Setup

This project sets up a development environment for a React web application using Docker. The web application displays an `<h1>` tag with the text "Codin 1" and runs on `localhost:7775`.

## Prerequisites

- Docker installed on your machine
- Node.js installed on your machine

## Setup Instructions
If you haven't already created a React application, you can use Create React App:

sh
Copy code
npx create-react-app .
Modify the App.js to display "Codin 1":

Edit the src/App.js file to include:

jsx
Copy code
import React from 'react';

function App() {
  return (
    <div className="App">
      <h1>Codin 1</h1>
    </div>
  );
}

export default App;
Build the Docker image:

sh
Copy code
docker build -t gill_kanwardeep_coding_assignment11 .
Run the Docker container:

sh
Copy code
docker run -p 7775:3000 -d --name gill_kanwardeep_coding_assignment11 gill_kanwardeep_coding_assignment11
Access the web application:

Open your web browser and go to http://localhost:7775 to see the "Codin 1" website.