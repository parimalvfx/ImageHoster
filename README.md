# ImageHoster

Image hosting website similar to Imgur

#### Part A - Fixing Issues

##### User signup bugs

* Check added in UserController class for username validation at the time of registration. If username is not available then error is added which will be flashed promptly on registration page:

    ![Error flashed on registration page if username is not available](docs/part_a_username_not_available.png)
