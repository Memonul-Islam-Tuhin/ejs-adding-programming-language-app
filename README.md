# 🚀 EJS Adding Programming Language App


A simple **Node.js + Express + EJS** web application where users can add and display programming languages dynamically.

This project demonstrates:
- Express server setup
- EJS templating
- Form handling
- Basic dynamic rendering

---

# 📌 Table of Contents

- 📖 About the Project  
- ✨ Features  
- 🛠️ Technologies Used  
- 📸 Screenshots  
- 💻 Installation  
- ▶️ How to Run  
- 📁 Project Structure  
- 📚 How It Works  
- 🤝 Contributing  
- 📜 License  

---

# 📖 About the Project

This is a beginner-friendly Express + EJS project.

Users can:
- View a list of programming languages
- Add new languages through a form
- See updates instantly rendered on the page

It is perfect for learning:
- Express routing
- EJS templating
- Handling POST requests
- Rendering dynamic content

---

# ✨ Features

✔️ Add programming languages  
✔️ Display dynamic list  
✔️ EJS template rendering  
✔️ Express routing  
✔️ Clean project structure  

---

# 🛠️ Technologies Used

- **Node.js**
- **Express.js**
- **EJS (Embedded JavaScript)**
- **HTML5**
- **CSS3**
- **JavaScript**

---

# 📸 Screenshots

## 🏠 Home Page
_Add a screenshot and name it `home.png` inside a `screenshots` folder._

```md
![Home Screenshot](./screenshots/home.png)
```

## ➕ Add Language Page
_Add a screenshot and name it `add.png` inside a `screenshots` folder._

```md
![Add Screenshot](./screenshots/add.png)
```

(Create a folder named `screenshots` and place your images there.)

---

# 💻 Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Memonul-Islam-Tuhin/ejs-adding-programming-language-app.git
```

### 2️⃣ Navigate into the Project Folder

```bash
cd ejs-adding-programming-language-app
```

### 3️⃣ Install Dependencies

```bash
npm install
```

---

# ▶️ How to Run

Start the server:

```bash
npm start
```

OR (if no start script is defined):

```bash
node index.js
```

Now open your browser and go to:

```
http://localhost:3000
```

*(Change the port if your app uses a different one.)*

---

# 📁 Project Structure

```
ejs-adding-programming-language-app/
│
├── public/               # Static files (CSS, JS)
├── views/                # EJS template files
│   ├── index.ejs
│   └── add.ejs
│
├── index.js              # Main server file
├── package.json
├── package-lock.json
├── .gitignore
└── README.md
```

---

# 📚 How It Works

### 🧠 Server Setup

- Express initializes the server
- EJS is set as the view engine
- Static files served from `public` folder

### 🛣️ Routes Example

```js
app.get("/", (req, res) => {
  res.render("index", { languages });
});

app.post("/add", (req, res) => {
  const newLanguage = req.body.language;
  languages.push(newLanguage);
  res.redirect("/");
});
```

### 🖼️ EJS Example

```ejs
<ul>
  <% languages.forEach(function(language){ %>
    <li><%= language %></li>
  <% }) %>
</ul>
```

---

# 🤝 Contributing

Want to improve this project?

1. Fork the repository  
2. Create a new branch  
   ```bash
   git checkout -b feature-name
   ```
3. Commit changes  
   ```bash
   git commit -m "Added new feature"
   ```
4. Push to GitHub  
   ```bash
   git push origin feature-name
   ```
5. Open a Pull Request  

---

# 📜 License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute it.

---

# 🙌 Author

**Memonul Islam Tuhin**

If you like this project, consider giving it a ⭐ on GitHub!

---
