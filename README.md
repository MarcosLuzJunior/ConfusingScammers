# ConfusingScammers
The script will try to simulate an user entering its own details into a malicious website

# How?
- The script will guide create a fake password and email account with the extension of choice 
- You can add a phone extension using the random library, in this instance it was not needed but if you need one here's a way you could do it 
    ""Generate random telephone number
    first = str(random.randint(100, 200))
    second = str(random.randint(1, 999)).zfill(3)
    third = str(random.randint(1, 888)).zfill(3)
    number = '+4407' + '{}{}{}'.format(first, second,third)""
    
- Finally using the requests library, the user will POST to the URL of choice the made up user name, email address and also possibly a telephone number

#Note:
Most of these website have a front site which has a link that redirects the information to a different website. In order to identify which URL to use have a look at this link: (https://developers.google.com/web/tools/chrome-devtools/network)
