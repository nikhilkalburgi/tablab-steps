# Clone our GitHub repository before starting

* First, navigate to [tablab-steps][1] repository and click the "Fork" button. This creates a personal copy of the repository under your GitHub account.
* Then, open your terminal and run the following command, replacing `username` with your actual GitHub username:

  ```bash
  git clone https://github.com/<username>/tablab-steps.git
  ```

* Afterwards, you can optionally add the original repository as an upstream remote to keep your fork updated:

  ```bash
  git remote add upstream https://github.com/samus-io/tablab-steps.git
  ```

* Before making changes, switch to a new branch to keep your work organized, the branch structure we defined is `lab/<lab-name>` or if you want to commit one Step `step/<step-name>`:

  ```bash
  git checkout -b lab/java-sqli
  ```

* Next, every time you want to save your Steps in your repository, execute:

  ```bash
  git add .
  git commit -m "Add new Steps about <Lab>"
  git push origin lab/java-sqli
  ```

* Finally, go to your fork on GitHub. Click `New pull request` near your branch, then review your changes. Once ready, submit your pull request with a detailed title and description, explaining what Steps you've added.

## Repository content

* Within [tablab-steps][1] repository, you'll discover a variety of resources designed to streamline the Step creation process:
  * `steps`: This directory hosts the Steps currently published on tablab.io, serving as a valuable reference or starting point for your own creations.
  * `static`: Here, you'll find the images utilized within the Steps, a crucial component for enhancing the visual appeal and clarity of your content.
  * `scripts`: A collection of scripts is available to assist in the creation and customization of Steps, simplifying tasks that might otherwise be time-consuming or complex.
  * `.vscode`: For those who use Visual Studio Code to craft Steps, this folder contains recommended extensions and settings designed to optimize your development environment and workflow.
  * `.markdownlint.json`: To ensure consistency across all Steps, this JSON file provides guidelines for Markdown formatting, promoting a uniform structure that enhances readability and maintainability.
  * `.prettierrc.json`: Associated with the Prettier extension, this configuration file is instrumental in maintaining a consistent coding style across your projects, aiding in the readability and professionalism of your code.
* By familiarizing yourself with these resources and adhering to the established guidelines, you'll be well-equipped to contribute valuable Steps to the tablab.io platform, enriching the learning experience for all users.

[1]: https://github.com/samus-io/tablab-steps
