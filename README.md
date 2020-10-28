# Login-System-in-Django
Register and Login system in django via Social Accounts


## Features

* Login with Facebook (required https doesn't work on localhost)
* Login with Google (it's tricky tho)
* Forget Password

## Usage

#### In [settings.py](loginsystem/settings.py)


Add your email-id and password
```
EMAIL_HOST_USER = ''        # your email-id for smtp
EMAIL_HOST_PASSWORD = ''    # your password
```

#### To login with Google account

1. Login as a superuser

2. Run the server

3. Log in as admin

4. In sites under SITES, change example.com
    -   Domain name:    127.0.0.1:8000
    -   Display name:   127.0.0.1:8000
    -   Save

5. Add these details in Social applications whitch is under SOCIAL ACCOUNTS
    -   Provider:   Google
    -   Name:       (anything you want)
    -   Client id:  (your client from [Google console](https://console.cloud.google.com))
    -   Secret key: (your secret key from [Google console](https://console.cloud.google.com))
    -   Sites: 127.0.0.1:8000 -> Chosen sites
    -   Save

    same steps for Facebook

Note: For login with facebook, you need to navigate [Facebook Developers](https://developers.facebook.com/), but login via Facebook only work on HTTPS protocal therefore it will not work on localhost but you can use implement that for testing purpose it will show the error saying 'The app is not secure'.