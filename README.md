# Real-Time Currency Conversion Web Application

> Live exchange rates, instant conversions, and a clean responsive UI — built with pure JavaScript and REST APIs.

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-Visit_App-38bdf8?style=for-the-badge)](https://rishusinghal15.github.io/Real-Time-Currency-Conversion-Web-Application/)
[![GitHub Pages](https://img.shields.io/badge/Deployed_on-GitHub_Pages-181717?style=for-the-badge&logo=github&logoColor=white)](https://rishusinghal15.github.io/Real-Time-Currency-Conversion-Web-Application/)

![Tech](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Tech](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![Tech](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Tech](https://img.shields.io/badge/REST_API-FF6C37?style=flat-square&logo=postman&logoColor=white)
![Status](https://img.shields.io/badge/Status-Live-brightgreen?style=flat-square)

---

## 🌐 Live Demo

**[https://rishusinghal15.github.io/Real-Time-Currency-Conversion-Web-Application/](https://rishusinghal15.github.io/Real-Time-Currency-Conversion-Web-Application/)**

---

## 📌 What It Does

A fast, lightweight currency converter that fetches **live exchange rates** via REST API and converts between any two currencies instantly — no page reloads, no delays.

Built entirely with vanilla JavaScript — no frameworks, no libraries — demonstrating strong core JS fundamentals including async programming, DOM manipulation, and API integration.

### Key Features

- 💹 **Real-time exchange rates** — fetches live data via REST API on every conversion
- 🔄 **Currency swap** — instantly swap source and target currencies with one click
- ✅ **Input validation** — handles edge cases like empty inputs, invalid amounts, and API errors gracefully
- 🖥️ **Responsive UI** — works seamlessly across desktop, tablet, and mobile devices
- ⚡ **Optimized API calls** — async/await with debouncing to avoid unnecessary requests
- 🔃 **Dynamic DOM updates** — results update live without any page refresh

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | JavaScript (ES6+) |
| Markup | HTML5 |
| Styling | CSS3 |
| Data | REST API (Exchange Rate API) |
| Async | Fetch API, Async/Await |
| Deployment | GitHub Pages |

---

## 🚀 Getting Started

### Option 1 — Use the Live App

👉 **[https://rishusinghal15.github.io/Real-Time-Currency-Conversion-Web-Application/](https://rishusinghal15.github.io/Real-Time-Currency-Conversion-Web-Application/)**

No setup needed — open and convert!

---

### Option 2 — Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/rishusinghal15/Real-Time-Currency-Conversion-Web-Application.git
cd Real-Time-Currency-Conversion-Web-Application

# 2. Open in browser — no build step needed!
open index.html
# or just double-click index.html
```

> No dependencies, no npm install — pure HTML/CSS/JS runs directly in the browser.

---

## 📁 Project Structure

```
Real-Time-Currency-Conversion-Web-Application/
├── index.html        # App structure & layout
├── style.css         # Responsive styling
├── app.js            # Core logic — API calls, DOM updates, validation
└── README.md
```

---

## 💡 How It Works

```
User enters amount + selects source & target currency
        ↓
  Input validation — checks for valid number & currency selection
        ↓
  Fetch API calls Exchange Rate REST API (async/await)
        ↓
  Live rate data returned as JSON
        ↓
  Converted amount calculated and displayed via DOM update
        ↓
  User can swap currencies → repeat instantly
```

### Core Logic Snippet (concept)

```javascript
async function getExchangeRate(from, to) {
  const response = await fetch(`${API_URL}/${from}`);
  const data = await response.json();
  return data.conversion_rates[to];
}

async function convertCurrency() {
  const rate = await getExchangeRate(fromCurrency, toCurrency);
  const result = amount * rate;
  displayResult(result);
}
```

---

## 📈 Technical Highlights

- ⚡ **Zero dependencies** — built with pure vanilla JS, proving strong core fundamentals
- 🔄 **Dynamic DOM manipulation** — results render instantly without page reload
- 📱 **Cross-device compatible** — responsive layout tested across screen sizes
- 🛡️ **Input validation** — handles invalid inputs, empty fields, and API failures gracefully
- 🚀 **Optimized API calls** — avoids redundant requests for better performance

---

## 🔮 Future Improvements

- [ ] Historical exchange rate charts (last 7/30 days)
- [ ] Multi-currency comparison (convert 1 currency to 10 at once)
- [ ] Offline support with cached rates (PWA)
- [ ] Dark mode toggle

---

## 👨‍💻 Author

**Rishu Singhal**

[![Live App](https://img.shields.io/badge/Live_App-Visit-38bdf8?style=flat-square)](https://rishusinghal15.github.io/Real-Time-Currency-Conversion-Web-Application/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/rishu-singhal-267734285)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rishusinghal15)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:rishusinghal2404@gmail.com)

---

⭐ **If this helped you, consider giving it a star!**
