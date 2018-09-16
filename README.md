# ImageHoster

Image hosting website similar to Imgur

### Part A - Fixing Issues

#### User signup bugs

* Check added in `UserController` class for username validation at the time of registration. Also updated `signup.html` file with class for flashing error. If username is not available then error is added which will be flashed promptly on registration page.

    * Error flashed if username is taken by another user:

        ![Error flashed on registration page if username is not available](docs/part_a_username_not_available.png)

#### Image upload issues

* Updated `ImageService`, `ImageServiceImpl`, `ImageManager` and `ImageController` classes to get images by id and to show images by title and id. Also updated `home.html` file with title + id link.

    * Images can have same title:

        ![Images now can have same title](docs/part_a_same_image_title.png)

    Above three images with title _abc_ resolves to following URLs:

    ```
    http://localhost:8080/images/abc/3
    http://localhost:8080/images/abc/4
    http://localhost:8080/images/abc/5
    ```

### Part B - Implement  a new feature

#### Username and password validity

* Check added for validity and length of the username and password fields upon user signup.

    * Username has been registered:

        ![Username has been registered](docs/part_b_username_registered.png)

    * Username needs to be 6 characters or longer:

        ![Username needs to be 6 characters or longer](docs/part_b_short_username.png)
    
    * Password needs to be 6 characters or longer:

        ![Password needs to be 6 characters or longer](docs/part_b_short_password.png)
