# Login-System-in-Django
Simple register and login system in django


## Features

* Login with GitHub
* Login with Facebook (required https doesn't work on local host)
* Login with Twitter
* Login with Google (it's tricky tho)
* Forget Password

## Usage

In [settings.py](loginsystem/settings.py)

```
# forget password
EMAIL_HOST_USER = ''        # your email-id for smtp
EMAIL_HOST_PASSWORD = ''    # your password
```

```
# for login with social media accounts
SOCIAL_AUTH_FACEBOOK_KEY = ''
SOCIAL_AUTH_FACEBOOK_SECRET = ''

SOCIAL_AUTH_TWITTER_KEY = ''
SOCIAL_AUTH_TWITTER_SECRET = ''

SOCIAL_AUTH_GITHUB_KEY = ''
SOCIAL_AUTH_GITHUB_SECRET = ''
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
    -   Secret key: (your secret key from[Google console](https://console.cloud.google.com))
    -   Sites: 127.0.0.1:8000 -> Chosen sites
    -   Save
