# Band-name-generator

A fun little web app that generates a band name based on your street name and your pet’s name! Built using **Express.js** and a custom **middleware function**.

---

## 📦 What It Does

- Accepts input from a form: street name + pet name
- A custom middleware combines them to form a band name
- Displays the generated band name on screen

---

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**
- **Body-Parser**
- HTML (served using `res.sendFile()`)

---

## 🚀 Getting Started

### 🔧 Installation

1. Clone this repo:
bash
git clone https://github.com/your-username/band-name-generator.git
2. Navigate into the folder:
bash
cd band-name-generator
3. Install dependencies:
bash
npm install
4. Run the server:
bash
node index.js
🔄 Make sure you’re using Node.js v14+ and running with ES modules enabled (use "type": "module" in package.json).


### 🌐 How to Use
1. Open your browser and go to:
http://localhost:3000/
2. Fill in your:
Street name
Pet name
3. Submit the form
Your band name will be displayed!
Example:
Your band name is:
BakerFluffy

### 📁 Project Structure

band-name-generator/
├── public/
│   └── index.html           # HTML form for input
├── index.js                 # Main Express server code
├── package.json             # Project config and dependencies
└── README.md                # Project documentation

### 🧠 How It Works
✅ Middleware
The custom middleware function bandnamegenerator takes the street and pet fields from the form, combines them, and stores the result in a variable.

function bandnamegenerator(req, res, next) {
  bandname = req.body["street"] + req.body["pet"];
  next();
}
It runs before the route that sends back the band name.

### 📦 Dependencies
-> express
-> body-parser

🎉 Have fun generating your band name!
