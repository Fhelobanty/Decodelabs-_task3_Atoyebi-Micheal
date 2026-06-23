# 🚀 CI Pipeline for Website Validation

## 📌 Overview

This project demonstrates a **Continuous Integration (CI) pipeline** using GitHub Actions to automate validation of a simple web project.

The pipeline is triggered on every push to the `main` branch and ensures that essential project files are present before changes are accepted.

---

## 🎯 Objectives

* Implement a CI pipeline using GitHub Actions
* Automate validation of project structure
* Simulate real-world DevOps workflow practices
* Gain hands-on experience with CI concepts

---

## 🛠️ Tech Stack

* GitHub Actions
* YAML
* HTML
* Bash (Shell Scripting)

---

## 🔄 Pipeline Workflow

The pipeline runs automatically on every push to the `main` branch.

### Steps:

1. **Checkout Repository**
   Clones the repository into the runner environment

2. **Validate HTML File**
   Checks if `index.html` exists

   * Passes if found
   * Fails if missing

3. **Success Confirmation**
   Displays a success message after validation

4. **List Files**
   Outputs repository contents for verification

---

## ⚙️ Validation Logic

```bash
if [ -f index.html ]
then
  echo "HTML file found"
else
  echo "HTML file missing"
  exit 1
fi
```

---

## 📸 Screenshots

### 1st pipeline workflow
<img width="1920" height="532" alt="Intenship 1 ci" src="https://github.com/user-attachments/assets/fb6027d8-9244-4551-a426-82aebea126f6" />

### Pipeline Success
<img width="1063" height="624" alt="Intenship 1 cii" src="https://github.com/user-attachments/assets/d56830f8-2900-4a5b-8783-e6fb04cea952" />

### Updated pipeline run
<img width="1637" height="610" alt="Intenship 1 ci-cd" src="https://github.com/user-attachments/assets/2e7f0618-bc67-41cd-9a7c-f884804e6c81" />

### Updated pipeline Success message
<img width="947" height="616" alt="Intenship 1 ci-cdd" src="https://github.com/user-attachments/assets/6f6e1d21-4be1-4e76-b853-89d20b93ef07" />

### Whole pipeline workflow
<img width="1273" height="422" alt="Intenship 1 ci-cd workflow" src="https://github.com/user-attachments/assets/27ebc90a-09bc-41ae-a1aa-fe0fa588ea16" />

### Pipeline YML
<img width="1018" height="824" alt="Intenship 1 pipeline yml" src="https://github.com/user-attachments/assets/93da52e5-68fa-4088-8076-6e2f4a7c8d9f" />




---

## 📂 Project Structure

```
.
├── .github/
│   └── workflows/
│       └── pipeline.yml
├── index.html
└── README.md
```

---

## 🚧 Future Improvements

* Add build stage
* Integrate automated testing
* Implement deployment (CI/CD)
* Deploy to AWS or GitHub Pages
* Add Docker support

---

## 🧠 Key Learnings

* Understanding CI pipeline structure
* Automating workflows with GitHub Actions
* Writing basic validation scripts
* Improving DevOps workflow practices

---

## 👨‍💻 Author

**Atoyebi Micheal Ademola**
DevOps Engineer intern DecodeLabs

---

##  Note

This project is part of a my hands-on DecodeLabs DevOps Internship journey focused on building practical CI/CD skills.
