# BCUContosotimetableAPI
Project to handle API testing by using POSTMAN Collection
# 📚 BCU Postman Collection

This repository contains the **BCU Postman Collection**, which includes API endpoints for managing **courses**, **events**, and **students**. These endpoints support pagination, item retrieval by ID, and updating item names.

---

## 🛠 Setup Instructions

### 1. Prerequisites
- [Postman](https://www.postman.com/downloads/) installed on your machine.
- (Optional) [Node.js](https://nodejs.org/) installed, for running via CLI using Newman.
- Internet access if you're testing against an external server.

---

## 📥 Importing the Collection in Postman

1. Open **Postman**.
2. Click on **Import** > **Upload Files**.
3. Select the file: `BCU.postman_collection.json`.
4. After import, open the collection and configure the following environment variable:

### 🔧 Environment Variables
- `Baseurl` → Set this to the base API URL, for example: https://localhost:57018
---

## 🚀 Running the Collection

### Option 1: Run in Postman
1. Open the **BCU** collection.
2. Click **Run Collection**.
3. Choose the environment where `Baseurl` is defined.
4. Hit **Run BCU** to execute all requests.

### Option 2: Run via Newman (Command Line)
#### Install Newman globally (if not already)
```bash
npm install -g newman
```
#### Run the collection
```
newman run BCU.postman_collection.json --env-var "Baseurl=https://localhost:57018"
```