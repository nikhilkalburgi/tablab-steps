# Adding images into Steps

* Images provide powerful visual reinforcement of textual content, making complex concepts easier to understand. Including relevant images in steps can also improve retention of concepts.
* Images should directly support the content, help explain concepts, and make the Step more interactive and visually appealing.
* You can include images by placing them in the `/static/images/learning` directory and referencing them in your markdown.
* Here is an example of how to include an image in a Step:

![SQL Injection][1]

* This is the markdown format we use to reference images:

  ```markdown
  ...
  ![This is an image][1]
  ...
  [1]: /static/images/learning/image.png
  ```

[1]: /static/images/injection-sql.png
