# 🚀 Trello API Testing Project

A professional **API Testing portfolio project** for entity["company","Trello"] covering **manual API testing, Postman test automation scripts, bug reporting, and end-to-end workflow validation**.

This repository demonstrates a real QA mindset through:

* Functional API validation
* Positive and negative test scenarios
* Business workflow coverage
* Defect reporting
* Automated Postman assertions
* Dynamic variable chaining

---

# 📌 Project Overview

This project validates core Trello workflows using **Postman Collections** and **manual test design techniques**.

The testing scope includes:

* Boards
* Lists
* Cards
* Checklists
* Labels
* Members
* Custom Fields

The project is designed to simulate a **real-world QA process** from requirement validation to bug reporting and response verification.

---

# ✅ Testing Scope

## 🔹 Manual API Testing

* CRUD operation validation
* Request/response verification
* Positive scenarios
* Negative scenarios
* Boundary validations
* Error handling
* End-to-end business workflows

## 🔹 Automated Postman Test Scripts

Automated assertions were implemented using **JavaScript in Postman Scripts**.

### ✔ Automation Coverage

* Status code validation
* Response body validation
* Response time checks
* Header validation
* Dynamic variable chaining
* Environment & collection variables
* Negative assertions
* Full CRUD workflow validation

### 🧪 Sample Script

```javascript
pm.test("Status code is 200", () => {
    pm.response.to.have.status(200);
});

pm.test("Response time less than 1000ms", () => {
    pm.expect(pm.response.responseTime).to.be.below(1000);
});

const res = pm.response.json();
pm.collectionVariables.set("boardId", res.id);
```

---

# 📂 Project Structure

```text
📁 Trello-API-Testing-Project
 ┣ 📄 Trello Postman Collection.json
 ┣ 📄 Trello Environment.json
 ┣ 📄 Trello_API_TestCases_BugReports.xlsx
 ┣ 📄 README.md
```

---

# 🔄 Covered API Workflows

* Create board → update → delete
* Create list → move → get cards
* Create card → update → archive → delete
* Add checklist → create check item → convert to card
* Add member → remove member
* Add label → remove label
* Custom field creation and deletion

---

# 🐞 Bug Reporting

The project also includes **real defect documentation** with:

* Bug title
* Steps to reproduce
* Expected result
* Actual result
* Severity
* Priority
* Evidence / response payload

This highlights practical QA skills beyond request execution.

---

# 📊 Test Coverage Metrics

* **Total Requests Covered:** 100+
* **Modules Covered:** 7+
* **Positive Scenarios:** ✅
* **Negative Scenarios:** ✅
* **Automation Assertions:** ✅
* **Bugs Reported:** ✅

---

# 🛠 Tools & Technologies

* entity["software","Postman"]
* JavaScript
* REST API
* JSON
* Excel Test Documentation
* entity["company","GitHub"]

---

# 💼 Portfolio Value

This project is suitable for:

* Junior QA Engineer roles
* API Tester roles
* Manual Tester positions
* Entry-level Automation QA opportunities

It demonstrates both **manual testing fundamentals** and **automation scripting basics** in a business-relevant workflow.

---

# ▶️ How to Run

1. Import the Postman collection
2. Import the environment file
3. Add your Trello API credentials
4. Run requests individually or execute workflows in sequence
5. Review automated assertions in the **Tests** tab

---

# ⭐ Key Highlights

* Real-world API workflows
* Professional QA documentation
* Manual + automation hybrid project
* Portfolio-ready GitHub repository
* Strong recruiter visibility

---

# 📬 Author

**Ahmed Yosry**

QA Engineer | API Testing | Postman | Manual Testing | Bug Reporting
