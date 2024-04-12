# Writing format to follow and copyright restrictions

* Creating a Step on [tablab.io][1] is about delivering a concise, clear, and engaging learning experience. This guide focuses on the format and writing style essential for crafting an effective Step.

## Follow our writing style convention

* Use Markdown syntax for styling all writings.
* Describe concepts using bulleted lists with short, specific sentences, like this one.
* Every sentence should begin with a bullet point.
* Avoid long sentences. If needed, split them by meaning, concept or context.
* Avoid first-person sentences when explaining a concept, such as "Imagine you are running an online platform where...". Instead, the impersonal approach, like “It can be considered an online platform where..." should be used.

### Defining titles

* It's not necessary to add `:` to the end of a title to introduce the bulleted list.
* Do not use capital letters for words that do not represent a concept. For example, the title "Use Case" should simply be "Use case." However, when using "Input Validation" in a title, since it represents a concept by itself, we should opt for "Input Validation overview" in capital letters, for instance.

### Using emojis

* :writing_hand: (`writing_hand`): is used to indicate to the learner that a practical exercise follows.
* :older_man: (`older_man`): is used to explain some concept that is related to the Step but is not specifically covered.
* :warning: (`warning`): is used when the learner must pay attention to an important section.

### Adding a table

* You can add tables when necessary. To do so, keep in mind that this is the format that our Markdown render processes:

  ```markdown
  |Column 1|Column 2|Column 3|
  |:--:|:--:|:--:|
  |Field 1|Field 2|Field 3|
  |Field 4|Field 5|Field 6|
  ```

### Adding an image

* When you want to add an image to the content to explain a concept in a more representative way, you first need get the image on your computer and then place it as a static file in the `/static/images/` folder that you will find in this repository.
* Once done, you can embed the image following the Markdown code as shown:

  ```markdown
  ![Image caption here][1]
  ```

  Afterwards, you just need to reference it at the end of the file like this:

  ```markdown
  [1]: /static/images/your-selected-image.png
  ```
  
  Note that the image path `/static/images/your-selected-image.png` refers to the absolute path where the image has supposedly been placed in this repository.
* **Important notice**: you can add any image you want, even if you didn't create it yourself. We will be in charge of creating a new image that represents exactly the same concept but in corporate format (styles and colors) and avoiding any copyright infringement.

### Using Visual Studio Code

* For those using Visual Studio Code, you will find in this repository configurations for several plugins designed to enhance your Markdown writing experience.
* To install the recommended extensions for this project, please follow these steps in Visual Studio Code:
  1. Launch Visual Studio Code loading the [tablab-steps][2] repository.
  1. Navigate to the *Extensions* view by pressing `Ctrl+Shift+X` (or `Cmd+Shift+X` on macOS).
  1. Type `@recommended` into the search bar.
  1. Click on the install button adjacent to the extensions listed under *Workspace Recommendations*.

## Respect copyright

* As a content creator, it's crucial to understand and respect copyright laws, ensuring you do not use or replicate sentences or texts from other websites or material.
* Just exchanging words for similar meanings in a sentence, without making any changes to the sentence structure or grammar, is still recognized as a form of plagiarism.
* AI tools can assist you in content creation, but texts directly produced by artificial intelligence systems are not allowed on [tablab.io][1].

[1]: https://tablab.io
[2]: https://github.com/samus-io/tablab-steps
