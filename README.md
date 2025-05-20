# 🚀 Code X: Free Dashboard, Panel & Wings Installation 🚀

Welcome to Code X! We provide a streamlined guide for installing your Pterodactyl-like Dashboard, Panel, and Wings (Daemon) 24/7.

---

## 🚨 **IMPORTANT NOTICE: WATCH THE VIDEO GUIDE FIRST!** 🚨

**Before you begin any installation steps, it is CRITICAL that you watch the full video guide provided by the original developer.** This guide will walk you through the entire process and help you understand the configuration requirements.

**Original Project & Guide By: Dragon Labs**

**We strongly advise you to watch the full video first. Only then, if you encounter persistent issues, should you create a ticket in our Discord server for support.**

---

## ❓ **Having Issues? Get Support Here!**
Join our Discord community for assistance and to create support tickets:
🔗 **[https://dsc.gg/codexsupport](https://dsc.gg/codexsupport)**

---

## ✨ **Overview of Components**

This guide covers the installation of three core components:

1.  **Panel:** The web-based administration interface.
2.  **Daemon / Wings:** The server-side process that manages game servers.
3.  **Dashboard:** Your front-end interface for users.

---

## 📋 **Prerequisites**

Before you start, ensure your server meets these requirements:

* **Operating System:** A clean installation of Ubuntu (recommended) or Debian.
* **Root Access:** You need to be logged in as root or have `sudo` privileges.
* **Basic Tools:** `git`, `nodejs`, `npm`, `zip`, `curl`, `nano`.

---

## 🚀 **Getting Started: Installation Steps**

Follow these steps carefully for each component.

### **1. Panel Installation**

This sets up the core web panel for managing your servers.

1.  **Clone the Panel Repository:**
    ```bash
    git clone [https://github.com/dragonlabsdev/v2panel](https://github.com/dragonlabsdev/v2panel)
    ```
2.  **Install Node.js (Version 23.x Recommended):**
    ```bash
    curl -sL [https://deb.nodesource.com/setup_23.x](https://deb.nodesource.com/setup_23.x) | sudo bash -
    ```
3.  **Install Essential Packages:**
    ```bash
    apt-get update && apt-get install -y nodejs git zip
    ```
4.  **Navigate to Panel Directory:**
    ```bash
    cd v2panel
    ```
5.  **Extract & Enter Panel Subdirectory:**
    ```bash
    unzip panel.zip && cd panel
    ```
6.  **Install Dependencies, Seed Database, and Create Admin User:**
    ```bash
    npm install && npm run seed && npm run createUser
    ```
    *(Follow the prompts to create your admin user credentials.)*
7.  **Start the Panel:**
    ```bash
    node .
    ```

---

### **2. Daemon / Wings Installation**

This component allows your Panel to communicate with and manage game servers.

1.  **Clone the Daemon Repository:**
    ```bash
    git clone [https://github.com/draco-labes/draco-daemon](https://github.com/draco-labes/draco-daemon)
    ```
2.  **Navigate to Daemon Directory:**
    ```bash
    cd draco-daemon
    ```
3.  **Install Dependencies:**
    ```bash
    npm install
    ```
4.  **Configure DracoDaemon:**
    ```bash
    node .
    ```

---

### **3. Dashboard Installation**

The Dashboard provides the user-facing interface for your clients.

1.  **Clone the Dashboard Repository:**
    ```bash
    git clone [https://github.com/dragonlabsdev/dashboard-v1.0.0](https://github.com/dragonlabsdev/dashboard-v1.0.0)
    ```
2.  **Navigate to Dashboard Directory:**
    ```bash
    cd dashboard-v1.0.0
    ```
3.  **Install Dependencies:**
    ```bash
    npm install
    ```
4.  **Prepare Environment Configuration:**
    ```bash
    mv .env_exemple .env
    ```
5.  **Edit Environment Variables:**
    ```bash
    nano .env
    ```
6.  **Start the Dashboard:**
    ```bash
    node .
    ```

---


## 💖 **Credits**
This installation guide is provided by **Code X**.
All core components (Panel, Daemon, Dashboard) are originally developed by **Dragon Labs**.
We extend our gratitude for their hard work and contributions to the community.
