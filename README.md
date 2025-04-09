# JulesApiAutomation

# 🚀 Jules API Test Automation with Postman + Newman + HTMLExtra Report

This project demonstrates how to automate API testing using **Postman**, execute collections with **Newman**, and generate detailed HTML reports using the **newman-reporter-htmlextra**.

---

## 📂 Project Structure

. ├── Postman/ │ ├── .github/ │ └── workflows/ │ └── gitActions.yml ├── newman/ │ └── report.html (generated) └── README.md


---

## ✅ Prerequisites

- [Node.js](https://nodejs.org/) installed

### 🔧 Install Newman and HTMLExtra Reporter

Use the following command to install Newman and the `htmlextra` reporter globally:

```bash
npm install -g newman newman-reporter-htmlextra
newman --version

newman run ./Postman/JulesApiAutomation.postman_collection.json \
  -r htmlextra \
  --reporter-htmlextra-export ./newman/report.html
