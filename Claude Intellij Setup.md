# Enabling Claude AI in IntelliJ

This guide explains how to enable and configure **Claude AI** inside **IntelliJ IDEA** using the MCP Server and required plugins.

---

## **Prerequisites**
Before starting, ensure you have the following installed:

- **IntelliJ IDEA v25 or later**
- **Claude Desktop**
- **Node.js v18 or later**

---

## **Setup Steps**
Follow these steps in order:

### **1. Download Claude Desktop**
Download and install Claude Desktop from the official site:

https://www.claude.com/download

---

### **2. Log in to Claude Desktop**
Open the Claude Desktop application and log in to your account.

---

### **3. Install the MCP Server Plugin in IntelliJ**
1. Open **IntelliJ IDEA**.
2. Navigate to **Settings → Plugins**.
3. Search for **MCP Server**.
4. Click **Install**.

---

### **4. Edit Claude Developer Config**
1. In Claude Desktop, go to:
   **Settings → Developer → Edit Config**.
2. This will open the `claude_desktop_config.json` file.
3. Open the file using **Notepad++**.
4. Ensure the JSON file is **empty**.
5. Save the file.

---

### **5. Fully Close Claude Desktop**
Close Claude Desktop completely.

- Make sure no Claude processes are running in **Task Manager**.

---

### **6. Enable the MCP Server in IntelliJ**
1. Go back to **IntelliJ**.
2. Open **Settings → Tools → MCP Server**.
3. Enable **MCP Server**.
4. Click **Auto Configure**.
5. Apply and select **OK**.

---

### **7. Re-open Claude Desktop**
Open Claude Desktop again.

---

### **8. Verify JetBrains Config in Claude**
Go to:
**Settings → Developer**

You should now see a **JetBrains configuration** generated automatically.

---

### **9. Install the Claude Plugins in IntelliJ**
1. In IntelliJ, open **Settings → Plugins**.
2. Search and install:
   - **Claude Code**
   - **Claude Code Terminal**

---

### **10. Install Claude Code CLI (Required for Access in IntelliJ)**
Open the **IntelliJ Terminal** and run:

```sh
npm install -g @anthropic-ai/claude-code
```

> Note: A **Claude subscription** is required to use Claude Code directly inside IntelliJ.

---

## **Setup Complete**
Claude AI should now be fully integrated and ready to use within IntelliJ IDEA.

