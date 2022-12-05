# chatgpt-terminal-test
This is a headless chrome based API that can run on your localhost and you can test via terminal, Thunderclient, Postman etc

This repository has been inspired by <a href="https://github.com/danielgross/whatsapp-gpt">whatsapp-gpt</a> by <a href="https://github.com/danielgross">Daniel Gross</a>

<h3>How to run:</h3>

```
git clone https://github.com/ayushgml/chatgpt-terminal-test.git
cd chatgpt-terminal-test
virtualenv pyenv
source pyenv/bin/activate
pip install -r requirements.txt
python server.py
```

Now in your terminal you can paste this sample curl request (or you can create your own):
```
curl -XGET http://localhost:5001/chat\?q\=i%20am%20having%20an%20exam%20tomorrow%20Any%20advice\?
```

<h4>The result should be like this:</h4>
<img width="1089" alt="chatgpt-ss" src="https://user-images.githubusercontent.com/72748253/205528340-aafc2d07-2928-4ead-9d45-bae47ab75883.png">

Note: the server.py code uses a sleep time for 15 seconds. So the content that can be processed by the chatGPT in 15 seconds can be seen in the terminal. Response message till 15 minutes will be recorded.

Although you can increase/derease the sleep time on line number 40 of server.py code.
