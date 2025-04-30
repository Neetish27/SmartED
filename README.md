SmartED is a smart educational platform designed to streamline digital learning and simplify administrative tasks for students and teachers.

---

CI/CT/CD Pipeline Flow

Our project follows a CI/CT/CD flow using **Jenkins**, **GitHub**, **Maven**, and **Docker**.

Pipeline Stages:

1. CI (Continuous Integration):
   - Code is pushed to GitHub.
   - Jenkins checks out the repository and triggers the pipeline.
   - Maven builds the project and runs unit tests.
     
2. CT (Continuous Testing):
   - JUnit or other test frameworks are triggered automatically in the Jenkins pipeline.
     
3. CD (Continuous Deployment):
   - On successful build, Docker image is built.
   - Image is pushed to Docker Hub.
   - Container is deployed locally or to a staging environment.


Setup & Run Instructions

1. Clone the repo
   
```bash
git clone https://github.com/Neetish27/SmartED.git
cd SmartED

Build the project - mvn clean install
Run the application - python3 app.py

Or using Docker:- docker build -t smarted-app .
                  docker run -p 5000:5000 smarted-app
```
Team Members and Responsibilities
Neetish Dhavgaye (22101A0007) - Dockers and Git
Mrugank Vichare (22101A0006) - Jenkins and Git
