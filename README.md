# Django ToDo list

This is a todo list web application with basic features of most web apps, i.e., accounts/login, API, and interactive UI. To do this task, you will need:

- CSS | [Skeleton](http://getskeleton.com/)
- JS  | [jQuery](https://jquery.com/)

## Explore

Try it out by installing the requirements (the following commands work only with Python 3.8 and higher, due to Django 4):


```
pip install -r requirements.txt
```

Create a database schema:

```
python manage.py migrate
```

And then start the server (default is <http://localhost:8000>):

```
python manage.py runserver
```

Now you can browse the [API](http://localhost:8000/api/) or start on the [landing page](http://localhost:8000/).

## Task

Extend a GitHub Actions workflow for this project with a Docker build and push to the DockerHub Registry.
Docker CI Job Requirements:

1. Update your forked repository with your DockerHub username and password.
    1. Add Corresponding secrets to the repository.
2. Update DockerImageName with your DockerHub image repository name
3. Use Matrix to run unit tests on different Python versions (3.8, 3.9).
4. Use Matrix to run unit tests on different OS types: ubuntu and windows.
5. Add input variables
    1. Input variable to choose which artifact from the matrix to deploy. (windows-3.8, ubuntu-3.9, etc)
6. Add branch protection to the main branch in your fork.
7. Add mandatory pull request and Python CI job status checks for PRs.
8. Add Manual Approval for STG environment.
9. Allow to run only one workflow per pull request.
10. New runs should cancel the previous runs.
11. Create a Pull Request with the changes.
12. Pull Requests description should also contain a reference to a workflow run with successfull workflow execution.
