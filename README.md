# 🚀 Free Dashboard + Panel + Wings Installation 24/7 By Code X 🚀

## 🚨 IMPORTANT! PLEASE READ BEFORE STARTING 🚨
**Before attempting any installation, we highly recommend watching the full video guide provided by the original owner.**
**Original Owner: Dragon Labs**

**Watch the full guide first, then if you encounter any issues, please create a ticket in our Discord server.**

## Need help? Join our Discord!
[https://dsc.gg/codexsupport](https://dsc.gg/codexsupport)
If you encounter any issues, please create a ticket in our Discord server for support.

---

## 💻 Installation Guides

### Panel Installation

1.  **Clone the repository:**
    `git clone https://github.com/dragonlabsdev/v2panel`
2.  **Install Node.js (v23.x):**
    `curl -sL https://deb.nodesource.com/setup_23.x | sudo bash -`
3.  **Install required packages:**
    `apt-get install nodejs git`
4.  **Navigate to the panel directory:**
    `cd v2panel`
5.  **Unzip and enter the panel directory:**
    `apt install zip -y && unzip panel.zip && cd panel`
6.  **Install dependencies, seed database, and create a user:**
    `npm install && npm run seed && npm run createUser`
7.  **Start the Panel:**
    `node .`

---

### Daemon / Wings Installation

1.  **Clone the repository:**
    `git clone https://github.com/draco-labes/draco-daemon`
2.  **Navigate to the daemon directory:**
    `cd draco-daemon`
3.  **Install dependencies:**
    `npm install`
4.  **Configure DracoDaemon (refer to documentation/prompts during execution):**
    *(You may be prompted for configuration details after running the next step)*
5.  **Start the Daemon:**
    `node .`

---

### Dashboard Installation

1.  **Clone the repository:**
    `git clone https://github.com/dragonlabsdev/dashboard-v1.0.0`
2.  **Navigate to the dashboard directory:**
    `cd dashboard-v1.0.0`
3.  **Install dependencies:**
    `npm install`
4.  **Rename environment example file:**
    `mv .env_exemple .env`
5.  **Edit environment variables (important for configuration):**
    `nano .env`
6.  **Start the Dashboard:**
    `node .`
