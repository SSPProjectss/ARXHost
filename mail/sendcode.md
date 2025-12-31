mini wiki for https://github.com/SSPProjectss/ARXHost/blob/main/mail/sendcode.html

The email is an html file. You can redo the page, options with metrics, backdoors or other malicious code are not allowed!
example
```
<html lang="ru">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>NAME</title>
</head>
<body style="background:white;color:black;">
<p>Hey, its mail</p>
</body>
</html>
```
<img width="302" height="178" alt="Снимок экрана 2025-12-31 в 3 37 13 PM" src="https://github.com/user-attachments/assets/d8016773-df1e-4603-82e7-05fed013258b" />

To display special information, use the available placeholders.
</br>
placeholders:
LOGIN: `${login}`
EMAIL: `${mail}`
CODE: `%s`


Possible types of authorization codes:
- One-time
- Link
to display the link and not the code, add `<a href="%s"> </a>` instead of the usual string `<div>%s</div>` as indicated in the original(https://github.com/SSPProjectss/ARXHost/blob/main/mail/sendcode.html). Yes, that's how the system works so far.

At the moment, you can only use a different letter to display a different language. To understand the language change system, use the `<html lang="LANG">` parameter (in head html). Yes, that's how the system works so far.
