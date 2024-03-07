# How to create a practical training exercise in a Step

* A Step can contain more than one exercise. The only thing to consider is that they must all be provided by the same containerized application.

## First, create a web app that provides the exercise(s)

* For any type of exercise you want to create, make sure to create an application that can be executed in [Cloud Run][1] on Google Cloud Platform. This is where our docker images are instantiated when a user deploys a Lab.
* Regardless of the number of exercises your application offers, make sure that it always offers them in the following way according to the order in which they are intended to be displayed within the content:
  * `/0/`: when the application is requested for this path, it should display the first exercise (even if there is only one).
  * `/1/`: when the application is requested for this path, it should display the second exercise.
  * `/2/`: when the application is requested for this path, it should display the third exercise.

## Second, build a Docker image

* Use the `docker` folder created in your Step structure. You should place inside this directory the application, which must be containerized.
* Write in the `Dockerfile` file the instructions to generate the Docker image.
* Note that the base image of the `Dockerfile` must be an official image from the [Docker Hub][2]. If you need an image that is not official, [contact the tablab.io team][3] and they will provide it for you.

## Third, include the exercise(s) in the content

* When you want to add an exercise at some point in the content of the Step, just add the following special tag:

  ```markdown
  @@ExerciseBox@@
  ```

  * For the first `@@ExerciseBox@@` tag typed, our platform, when processing the content, will request the path `/0/` to the application trying to reach the first exercise to be displayed.
  * For the second `@@ExerciseBox@@` tag found in the content, the path `/1/` will be requested in order to display the second exercise.
  * For the third `@@ExerciseBox@@` tag found in the content, the path `/2/` will be requested in order to display the third exercise.

## Last, but not least

* Please note that all submitted steps will be reviewed by the tablab.io team and we will make changes and corrections if the submitted steps do not follow the proper format.
* Remember that our mission is to make tablab.io a collaborative academy, so you can be sure that you will have our full support in the Step generation process. For any questions or improvements just [contact us][3], we are willing to help you with anything.

[1]: https://cloud.google.com/run
[2]: https://hub.docker.com/search?q=&image_filter=official
[3]: hello@samus.io
