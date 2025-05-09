# 📊 Cricket Players Stats API ⚡️

Welcome to the **Cricket Players Stats API**! 🎉 This API provides structured data for Indian cricket players, including detailed stats and image URLs. Whether you're building an app, visualizing stats, or just exploring data, this API has you covered! 🏏

---

## 🚀 Getting Started

### Step 1: Use the API URL

No setup is required! This API is publicly available and ready to be used via:

🔗 https://dakshgarg1311.github.io/API/players.json


You can fetch this directly using JavaScript in any frontend app or testing environment.

---

## 📡 API Overview

This API returns a **JSON array** of player objects. Each object contains:

- `id` – Unique ID of the player
- `name` – Full name of the player
- `bowlingStyle` – Bowling average
- `wickets` – Total number of matches played
- `image_url` – Direct URL to player image

---

## 🛠️ How to Use (with JavaScript)

Here’s how you can fetch and use the data using `fetch` in JavaScript:

### 🧪 Basic Fetch Example

```javascript
fetch("https://dakshgarg1311.github.io/API/players.json")
  .then(response => response.json())
  .then(data => {
    console.log("All Players:", data);

    // Example: Display each player's name
    data.forEach(player => {
      console.log(`👤 ${player.name}`);
    });
  })
  .catch(error => {
    console.error("🚨 Error fetching player data:", error);
  });

# 🎯 Fetch a Specific Player by ID

const playerId = "12345";

fetch("https://dakshgarg1311.github.io/API/players.json")
  .then(response => response.json())
  .then(data => {
    const player = data.find(p => p.player_id === playerId);
    
    if (player) {
      console.log("🏏 Player Found:", player);
    } else {
      console.log("❌ Player not found.");
    }
  })
  .catch(error => {
    console.error("🚨 Error fetching player data:", error);
  });
```
 
💡 Features
✅ Full player profiles

🏏 Batting and bowling stats

🖼️ Player image URLs

⚡ Fast access via static JSON URL

💻 Easy integration with frontend apps

📬 Contact
Have questions, feedback, or want to collaborate?
📧 Reach out at: thedakshgarg@gmail.com


Let me know if you want a live preview badge, a React demo snippet, or a table of contents!
