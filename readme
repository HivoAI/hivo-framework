![Logo](https://docs.hivo.ai/~gitbook/image?url=https%3A%2F%2F2606891579-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FGEHVHcdT0adTfRfFAPoA%252Fuploads%252FGrfV7BGETpcttJyyVyUZ%252Fbg%2520%282%29.png%3Falt%3Dmedia%26token%3D1c535a4a-6044-4513-9975-aba0da3f7c74&width=376&dpr=2&quality=100&sign=48936ff9&sv=2)

# HivoAI Framework - AI Agents for Blockchain  

HivoAI is an **open-source framework** designed to simplify the **creation, deployment, and interaction** with AI-powered agents. With a **command-line interface (CLI)**, users can seamlessly manage AI-driven agents while leveraging **Solana blockchain** technology for decentralized automation.

---

## 🚀 Key Features
- **AI Agent Deployment** → Easily launch AI-powered agents onto the **Solana blockchain**.
- **Blockchain Data Fetching** → Get **market cap, top token holders, and trading statistics** in real-time.
- **Token & Trading Analysis** → Identify **trending tokens**, monitor transactions, and analyze token movement.
- **Advanced Query Execution** → Perform **custom blockchain queries** to extract valuable insights.
- **Seamless API Integration** → Built-in support for **Bitquery APIs** for extended blockchain data access.

---

## 🛠 Capabilities & Functionality  
- **Token Insights** → Retrieve **market cap, token supply, and holder details**.
- **Trading Pattern Detection** → Analyze **market movements and transaction volumes**.
- **Command-Line Execution** → Manage AI agents directly via **CLI commands**.
- **Cross-Platform Support** → Fully compatible with **modern JavaScript (Node.js) environments**.
- **Extensibility** → Modify and extend **existing AI agents** or create **custom agents**.

---

## 📌 Getting Started  

### **🔹 Prerequisites**  
Before using HivoAI, ensure you have:  
✔ **Node.js** (16.x or later)  
✔ **npm or yarn** installed  
✔ **Bitquery API Key** for blockchain data access  

---

### **🔹 Installation & Setup**  

1️⃣ **Clone the Repository**  
```bash
git clone https://github.com/hivoai/hivoai-framework-v1.git
cd hivoai-framework-v1
```

2️⃣ **Install Dependencies**  
```bash
npm install
```

3️⃣ **Configure Environment Variables**  
Create a `.env` file in the root directory and add:  
```bash
PRIVATE_KEYPAIR=<YOUR_PRIVATE_KEYPAIR>
OPENAI_API_KEY=<YOUR_OPENAI_API_KEY>
RPC_ENDPOINT=https://api.mainnet-beta.solana.com
```

4️⃣ **Build the Framework**  
```bash
npm run build
```

---

## 📜 Available Commands  

### **1️⃣ Ask AI Agents a Question**
```bash
npm run askhivo {agentName} {yourQuestion}
```
**Example:**  
```bash
npm run askhivo Nova "What is the market cap of Ethereum?"
```

### **2️⃣ Deploy an AI Agent**
- Modify `defineAgent.ts` to customize agent parameters.
- Then, execute:
```bash
npm run build
npm run deployhivo
```
- Deploys an AI agent to the Solana blockchain.

### **3️⃣ Interact with an AI Agent**
```bash
npm run interacthivo {agent_name} ask "Your question"
```
**Example:**  
```bash
npm run interacthivo Nova ask "Show me the top trending tokens in 24h"
```

### **4️⃣ Fetch Trending Tokens**
```bash
npm run interacthivo Nova ask "Trending tokens 24h"
```

### **5️⃣ Fetch Top Token Holders**
```bash
npm run interacthivo Nova ask "Top holders: {mintAddress}"
```
**Example:**  
```bash
npm run interacthivo Nova ask "Top holders: 6LKbpcg2fQ84Ay3kKXVyo3bHUGe3s36g9EVbKYSupump"
```

### **6️⃣ Fetch Market Cap Data**
```bash
npm run interacthivo Nova ask "Marketcap count:{count} term:\"{term}\""
```

### **7️⃣ Fetch First Top Buyers**
```bash
npm run interacthivo {agentName} ask "First top {count} buyers for: {mintAddress}"
```

### **8️⃣ Execute Token Trades**
```bash
npm run hivo-trade {agent_name}
```

---

## 🔧 Dependencies

| Dependency         | Version  | Description |
|--------------------|----------|-------------|
| `@solana/web3.js`  | ^1.98.0  | Solana blockchain interaction |
| `dotenv`           | ^16.4.7  | Loads environment variables |
| `firebase`         | ^11.1.0  | Secure data storage |
| `node-fetch`       | ^3.3.2   | API request handling |
| `openai`           | ^4.77.3  | OpenAI API for AI queries |
| `bs58`             | ^6.0.0   | Base58 encoding/decoding |

## 🛠 Development Dependencies

| Dependency         | Version  | Purpose |
|--------------------|----------|---------|
| `typescript`      | ^5.7.3   | Strongly-typed JavaScript |
| `ts-node`         | ^10.9.2  | Run TypeScript directly |
| `tsconfig-paths`  | ^4.2.0   | Simplifies module imports |

---

## 🔗 Using `api.hivo.ai` API  

### **1️⃣ Fetch Agent Details**
```bash
curl https://api.hivo.ai/api/agent/Nova
```

### **2️⃣ Interact with an AI Agent (GET)**
```bash
curl "https://api.hivo.ai/api/agent/Nova/interact?message=Hello!"
```

### **3️⃣ Interact with an AI Agent (POST)**
```bash
curl -X POST "https://api.hivo.ai/api/agent/Nova/interact" \
-H "Content-Type: application/json" \
-d '{"message": "Hello, Nova"}'
```

---

## 📌 Example Usage in Node.js  

```javascript
const fetch = require("node-fetch");

async function interactWithAgent(agentName, message) {
  const response = await fetch(`https://api.hivo.ai/api/agent/${agentName}/interact`, {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({ message }),
  });

  if (!response.ok) {
    console.error("Error:", response.statusText);
    return;
  }

  const data = await response.json();
  console.log("Agent Response:", data.reply);
}

interactWithAgent("Nova", "What are the top performing tokens today?");
```

---

## 🤝 Contributing  
Want to contribute? Follow these steps:  
1. **Fork the repository**  
2. **Create a feature branch** (`feature/my-new-feature`)  
3. **Commit and push your changes**  
4. **Submit a pull request**  

🔥 Happy coding with **HivoAI!** 🚀  
