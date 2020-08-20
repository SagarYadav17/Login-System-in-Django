# Login-System-in-Django
Simple register and login system in django from the [video](https://www.youtube.com/watch?v=tUqUdu0Sjyc) of Dennis Ivy's 

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

Then migrate and runserver
