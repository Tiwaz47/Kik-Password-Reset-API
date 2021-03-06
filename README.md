# Usage
`curl -X POST -d emailOrUsername=<EMAIL_OR_USERNAME_HERE> https://KPR-API.stethosayshello.repl.co`

![Curl_Example](https://cdn.discordapp.com/attachments/895908071107362836/919619092527325234/raw.gif)

Alternativley, two example projects are posted here, they're pretty self explanitory.

`git clone https://github.com/StethoSaysHello/Kik-Password-Reset-API` then run which one you want to try out.

[Text_Version.py](https://github.com/StethoSaysHello/Kik-Password-Reset-API/blob/main/Text_Version.py) is an example that can be used in the shell/terminal. ([Test it here!](https://replit.com/@StethoSaysHello/KPR-Text?v=1))

![Text_Version](https://cdn.discordapp.com/attachments/895908071107362836/919619131081363476/gif1.gif)

[GUI_Version.py](https://github.com/StethoSaysHello/Kik-Password-Reset-API/blob/main/GUI_Version.py) is an example with a simple windowed user interface. ([Test it here!](https://replit.com/@StethoSaysHello/KPR-GUI?v=1))

![GUI_Version](https://cdn.discordapp.com/attachments/895908071107362836/919619043265245224/gui.gif)

# Disclaimers
I return the raw response from [ws.kik.com/p](https://ws.kik.com/p), which tends to have some odd formatting, It's reccomended that you reformat it like I have in these examples before using it in your projects. At the moment rate limits still apply after 5-6 attempts, it'll just return the "invalid user/email" response, I'm working on ways to detect it so that I can [bypass it](https://stackoverflow.com/questions/55872164/how-to-rotate-proxies-on-a-python-requests/68451842#68451842). In addition, issues with Kik's password reset page going down or taking too long to respond are pretty frequent... _Suprise suprise, right?_

Source code is obfuscated and hosted myself to avoid abuse, **I can see all traffic, and fully intend on using that to add automatic blacklisting for IPs that spam multiple calls a second.** Though the source code will return error responses if you attempt to run it on an unauthorized machine, it does not contain harmful/malicious code of any kind.


