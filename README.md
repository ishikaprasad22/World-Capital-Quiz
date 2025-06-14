# 🌍 World Capital Quiz

A fun and interactive web quiz app built using **Node.js**, **Express**, **PostgreSQL**, and **EJS** — designed to test your knowledge of world capitals.

---

## 📸 Preview

> The app presents a random country  
> ➡️ You guess its capital  
> ✅ Get it right? Your score increases  
> 🔁 Next question appears instantly

---

## 🚀 Features

- Dynamic quiz from PostgreSQL database
- Real-time scoring
- EJS templated frontend
- Secure database config using `.env`

---

## 🛠️ Tech Stack

- Node.js  
- Express.js  
- PostgreSQL  
- EJS  
- body-parser  
- dotenv  
- nodemon (for development)

---

## 📁 Project Structure

```

World-Capital-Quiz/
│
├── public/             → Static files (CSS, images)
├── views/              → EJS templates
├── index.js            → Main server logic
├── capitals.csv        → Data for database
├── file.env            → Your local environment variables
├── .gitignore
├── package.json

````

---

## ⚙️ Local Installation Guide

> ⚠️ This section is for developers looking to run the project locally with their own database and environment setup.

### ✅ Prerequisites

Before you begin, make sure you have the following installed:

- [Node.js & npm](https://nodejs.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [Git](https://git-scm.com/)
- A terminal or CLI tool (e.g., PowerShell, bash, zsh)

### 🛠️ Steps

#### 1. Clone the Repository

```bash
git clone https://github.com/ishikaprasad22/World-Capital-Quiz.git
cd World-Capital-Quiz
````

#### 2. Install Dependencies

```bash
npm install
```

> 🔸 `nodemon` is included as a dev dependency and will be available via `npx`.

#### 3. Setup the PostgreSQL Database

* Create a new database named `world`
* Create a `capitals` table:

```sql
CREATE TABLE capitals (
  country VARCHAR,
  capital VARCHAR
);
```

* Import data into the `capitals` table (e.g., from `capitals.csv`)

#### 4. Configure Environment Variables

Create a file named `file.env` in the root of your project and add:

```
DB_USER=your_postgres_username
DB_HOST=localhost
DB_NAME=world
DB_PASSWORD=your_postgres_password
DB_PORT=5432
```

#### 5. Start the Server

```bash
npx nodemon index.js
```

Then open your browser and navigate to:
🌐 [http://localhost:3000](http://localhost:3000)

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♀️ Author

**Ishika Prasad**
GitHub: [@ishikaprasad22](https://github.com/ishikaprasad22)

