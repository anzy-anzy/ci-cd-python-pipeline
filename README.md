#  CI/CD Pipeline: Python App on AWS CodePipeline

This homework demonstrates a **2-stage CI/CD pipeline** using **GitHub**, **AWS CodePipeline**, and **CodeBuild**.  
The pipeline builds a simple Python application that prints my name.  

---

##  Homework Overview

- **Source Control:** GitHub  
- **CI/CD Orchestration:** AWS CodePipeline  
- **Build Tool:** AWS CodeBuild  
- **Runtime:** Python 3.9  
- **Application:** A simple Python script (`my_app.py`)  

---

##  Steps Followed

### 1. Create GitHub Repository
- Created a new repo: `ci-cd-python-pipeline`  
- Cloned repo locally and added two files:  
  - `my_app.py` → Python script that prints my name: print(" my name is Ebsiy Anslem") 
  - `buildspec.yml` → Instructions for CodeBuild.
  - push both files to github
    
 <img width="1920" height="933" alt="Screenshot (399)" src="https://github.com/user-attachments/assets/f712a327-935c-4b8a-b74c-fa95dad7187f" />


### 2. create my pipeline
- Source stage: github
- Build stage:
  Add a CodeBuild project.
- Configure it with:
  Managed image → Amazon Linux
  Runtime → Standard
  Buildspec → buildspec.yml (default)
  
 <img width="1920" height="942" alt="Screenshot (400)" src="https://github.com/user-attachments/assets/cae40a8e-e94a-434e-86e6-ba2f0514b135" />
 
### 3.CodeBuild log showing:

- Python version 
- Output: my name is Ebsiy Anslem
<img width="1920" height="982" alt="Screenshot (402)" src="https://github.com/user-attachments/assets/adf49965-800d-4ec7-af77-1991f9f6eca2" />

### Conclusion
 
- This homework demonstrated how to:
- Create and push code from GitHub to AWS CodePipeline.
- Configure CodeBuild with Python 3.9 runtime.
- Run a simple Python script (my_app.py) via CI/CD pipeline.
- Validate the build logs showing the expected output.
