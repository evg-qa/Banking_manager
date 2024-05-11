# Banking_manager_UI

#### Note:
The project was completed as part of participation in the SDET practicum, where one of the additional requirements was the ability to run in the CI/CD system. Because of this, it was decided to implement it in GitLab.

---
#### Project link:

[View project](https://gitlab.com/evge_qa/banking_manager)

#### Links to documentation:


[View task](https://gitlab.com/evge_qa/banking_manager/-/blob/main/documentation/task.md)

[View test cases](https://gitlab.com/evge_qa/banking_manager/-/blob/main/documentation/testcases.md)

[View Allure report](https://evge_qa.gitlab.io/-/banking_manager/-/jobs/6424598250/artifacts/allure-report/index.html)

---

### Running the project
#### Setup:
- Clone the repository to your computer:
```
git clone https://gitlab.com/evge_qa/banking_manager.git
```
- Navigate to the project's root folder

- Create a virtual environment:
```
python -m venv venv
```
- Activate the virtual environment:
  
Windows:
```
.\venv\Scripts\activate
```
macOS и Linux:
```
source venv/bin/activate
```

#### Dependencies:

- Install dependencies:
```
pip install -r requirements.txt
```

#### Running automated tests

- Run the command to execute tests:
```
pytest -s -v
```
- Run the command to execute tests in parallel:
```
pytest -s -v --dist loadgroup   
```

#### Generating and running Allure reports

- Run the command to execute tests:
```
pytest -s -v --alluredir allure-results
```
- Run the command to execute tests in parallel:
```
pytest -s -v --dist loadgroup --alluredir allure-results
```
- Run the command to view the report:
```
allure serve allure-results
```
