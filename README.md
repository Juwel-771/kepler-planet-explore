# Kepler Planet Explorer

A lightweight Node.js project that processes, filters, and analyzes NASA's Kepler mission dataset using JavaScript and the `csv-parse` library.

This project focuses entirely on **Node.js + JavaScript**, no frontend or additional frameworks. It reads the Kepler CSV data, extracts potentially habitable planets, and prints them in a clean and structured format.

---

## 🚀 Features

* 📁 Read large CSV data using streams
* 🔄 Efficient parsing with `csv-parse`
* 🪐 Filters out potentially habitable planets
* ⚡ Pure Node.js (no frameworks)
* 🧪 Beginner-friendly and clean code structure

---

## 🛠️ Tech Stack

| Layer         | Technologies                     |
| ------------- | -------------------------------- |
| **Runtime**   | Node.js                          |
| **Language**  | JavaScript                       |
| **Libraries** | csv-parse, fs (Node File System) |

---

## 📂 Project Structure

```
kepler-planet-explore/
├── data/
│   └── kepler_data.csv
├── src/
│   ├── index.js
│   └── planets.js
├── package.json
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```
git clone https://github.com/Juwel-771/kepler-planet-explore.git
cd kepler-planet-explore
```

### 2️⃣ Install Dependencies

```
npm install
```

### 3️⃣ Run the Project

```
node src/index.js
```

---

## 🧩 How It Works

1. Loads the Kepler CSV dataset
2. Parses each row as a JS object
3. Filters planets based on:

   * `koi_disposition === 'CONFIRMED'`
   * `koi_insol` within habitable range
   * `koi_prad` smaller than 1.6 Earth radii
4. Outputs final list of habitable planets in the console

---

## 📝 Example Output

```
Habitable planets found: 18
Kepler-62 f
Kepler-186 f
Kepler-442 b
...
All Done
```

---

## 📜 Scripts

```
npm start   # runs index.js
```

---

## 🤝 Contributing

PRs are welcome! If you want to improve filtering logic or add new analytics, feel free to open an issue.

---

## 📜 License

MIT License

---

## 👤 Author

**Juwel-771**
GitHub: [https://github.com/Juwel-771](https://github.com/Juwel-771)
