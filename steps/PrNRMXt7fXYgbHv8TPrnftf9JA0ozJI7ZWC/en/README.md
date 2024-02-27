# Run the helper script to create the directory structure

* Each Step within our system is uniquely identified by a `nanoid` and adheres to a specific directory structure designed to organize its content and functionalities efficiently:

  ```markdown
  Step
  ├── docker
  │   └── Dockerfile
  ├── es
  │   └── README.md
  ├── en
  │   └── README.md
  └── properties.json
  ```

* `en`: This directory is reserved for the Step's content, presented in Markdown format within the `README.md` files. The English version is essential, containing the Step's title as its first line following the syntax: `# <title>`.
* `es`: The Spanish counterpart, mirrors the English directory's structure, offering the Step's content in Spanish.
* `docker`: Central to the setup of each Step, the docker directory plays a crucial role in storing all the files required for building the exercise's Docker image. Within this directory, the Dockerfile will generate the Docker image. If a Step is designed without an accompanying exercise, then the docker folder should be left empty.
* `properties.json`: This JSON file contains the metadata of a Step, which outlines the number of exercises included, the anticipated completion time in minutes, and authorship details. The file's structure is as follows:

  ```json
  {
    "numExercises": 0,
    "estimatedCompletionTime": 0,
    "author": "samus.io",
    "authorGithubId": "samus-io"
  }
  ```

* By adhering to this structured approach, creators can ensure their Steps are both standardized and optimized for the best possible learning experience on tablab.io.

## [steps-helper][2] script

* To facilitate and streamline the Step creation process, we've developed the [steps-helper][2] script. This tool automates the generation of the necessary files, ensuring consistency and efficiency in Step development.
* To successfully run the script, it's essential to first set up the required dependencies. Begin this process by navigating to the `steps-helper` directory within scripts and initiating the installation of dependencies:

  ```bash
  cd ./scripts/steps-helper/
  npm install
  ```

* Following the installation, proceed by moving to the steps directory to execute the script:

  ```bash
  cd ../../steps
  node ../scripts/steps-helper/index.js
  ```

* Executing these commands will effectively generate the predefined structure for a Step. This structured approach ensures a streamlined setup, facilitating the creation of new Steps with ease.

[2]: /scripts/steps-helper/
