# How to create a practical training exercise

* A Step can contain more than one exercise, there is no limit. The only thing to consider is that the exercises will use the same docker image.
* When you want to add an exercise in the markdown, add the following:

  ```markdown
  * :writing_hand: Exercise statement
  @@ExerciseBox@@
  ```

* For each `@@ExerciseBox@@` tag there will be one exercise. As the exercises have the same image, the first will be in the route `/0/`, the second one at `/1/`, and so on.
* :writing_hand: Here you can see an example of an exercise:
  @@ExerciseBox@@

* Note that the base image of the `Dockerfile` must be an official image from the [Docker Hub][1]. If you need an image that isn't official, contact with the tablab.io team.
  * Using an official Docker image ensures that creators adhere to best practices, enhancing the reliability and quality of the exercises.

* Lastly, please note that all submitted steps will be reviewed by the tablab.io team and we will make changes and corrections if the Steps submitted doesn't follow our format.
* Dive into creating Steps on tablab.io and share your knowledge with the world! Your expertise can light the path of learning for others, turning every idea into an educational adventure. We are expecting you!

[1]: https://hub.docker.com/search?q=&image_filter=official
