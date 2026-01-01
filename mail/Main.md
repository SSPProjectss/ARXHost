The email is an html file. You can redo the page, options with metrics, backdoors or other malicious code are not allowed!
You can write letters yourself, the letter is an html page,if desired, you can use variables, only certain variables that you specify can be used in the letter, other variables will not work for safety purposes, below is a list of all available variables that we have in the project, if you want to add a new variablewrite to us in the ticket :).If you are thinking about multilingualism, write, at the moment, the other choice is to make another email with the change <html lang="LANG"> to another language that you want and the changes in the html file that you want. In order for your letter to be accepted into production, you must create an open github repository and add at least 2 files, 1 README file.MD with information about the letter, what you want to tell us, and MAIL.HTML is the letter itself. After that, you can open a ticket with the tag "Other" and the title "I want to add an email" and with any text and priority, and send a direct link to the repository in the ticket. Other options will rarely be considered.
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

To display special information, use the available placeholders. All possible codes are provided below, some codes do not work in some emails.
</br>
placeholders:
LOGIN: `${login}` user login (@user123)</br>
EMAIL: `${mail}` user email (user123@gmail.com)</br>
LINK: `${link}` any link in website system (google.com/auth/link/code=1234)</br>
TITLE: `${title}` title in mail</br>
BAR: `${h1}` bar in mail</br>
TEXT: `${p}` message in mail</br>
OTHER INFO: `${additionalInfo}` other informaiton in mail</br>
AUTH CODE: `%s` code in auth </br>
HALF IP: `${half_ip}` user ip (127.#.#.1)</br>
COUNTRY: `${country}` user country (USA)</br>
WARNING MESSAGE: `${warning}` user warning(warning! your account has performed a strange action)</br>
CRITICAL MESSAGE: `${critical}` user critical(warning! your account isyour account has performed a strange action)</br>
WARDEN SYSTEM DATA: `%warden_system_data%` user critical(warning! your account is hacked)</br>



Possible types of authorization codes:
- One-time
- Link
to display the link and not the code, add `<a href="%s"> </a>` instead of the usual string `<div>%s</div>` as indicated in the original(https://github.com/SSPProjectss/ARXHost/blob/main/mail/sendcode.html). Yes, that's how the system works so far.


At the moment, you can only use a different letter to display a different language. To understand the language change system, use the `<html lang="LANG">` parameter (in head html). Yes, that's how the system works so far.
