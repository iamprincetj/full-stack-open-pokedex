When working with python, some common steps in a CI setup include linting, testing, and building.

Linting is an essential step to ensure code quality and readability, in order for a developer to make use of this step he is going to use a tool. Selecting a linting is based on a developer’s needs, A developer can use Pylint which is used for rigorous linting in python and can be installed using: pip install pylint. Linters use configuration files to customize checks and make rules each python file must follow, create a config file e.g. .pylintrc to define rules and settings. Include a step in your CI/CD pipeline that runs the linter on your codebase. This ensures consistent checks and helps maintain code quality.

Testing is also a very important step as it’s used to write tests cases for individual functions and methods and ensures everything works as expected. One tool to use is python’s built in unittest framework for unit testing, integration testing to test interactions between components or modules. Integrate testing into your CI pipeline which runs test automatically whenever you push your code to your repository

Building in python could be using a requirement.txt file to list all python packages your project depends on which can be generated using pip freeze > requirement.txt

One alternative to Jenkins and Github Actions is Spacelift, it offers improved VCS integration, cloud-native support, and compatibility with GitOps workflows. It simplifies CI/CD setup and maintenance

This setup would be better in a cloud-based environment, this is because in its official site it says ‘Spacelift is simpler, offers improved visibility and compliance, and is easier to scale across different IaC providers and cloud platforms’. The fact that it’s easier to scale across cloud platforms make would make it better in a cloud-based environment.
