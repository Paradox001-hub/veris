VERIS — WEB VERSION
===================

Two files. That is all.

  veris.html   — open this in any browser
  server.py    — run this in Terminal first


SETUP
-----

1. Get your Anthropic API key
   Go to console.anthropic.com
   Create an API key if you don't have one

2. Set your API key (do this once per Terminal session)

   Mac:
     export ANTHROPIC_API_KEY=your_key_here

   Windows:
     set ANTHROPIC_API_KEY=your_key_here

3. Start the server

   Mac:
     python3 server.py

   Windows:
     python server.py

4. Open veris.html in your browser
   Double-click it, or drag it into a browser window

5. Enter your name and begin


EVERY TIME YOU USE IT
---------------------

1. Open Terminal
2. Navigate to the Veris folder:
     cd ~/Veris/web
3. Set your API key (if not already set)
4. Run: python3 server.py
5. Open veris.html in browser
6. When done, press Ctrl+C in Terminal to stop the server


SHARING WITH OTHERS
-------------------

Anyone on the same WiFi network can use Veris while your server is running.

Find your local IP address:
  Mac: System Settings > WiFi > Details > IP Address
  Windows: ipconfig in Command Prompt, look for IPv4 Address

Tell them to open: http://YOUR_IP:5000
Then send them the veris.html file, but change this line in it:
  fetch('http://localhost:5000/chat'
To:
  fetch('http://YOUR_IP:5000/chat'

Or just have them sit with you at your computer.


NOTES
-----

- Conversations are not saved between sessions (persistent memory coming later)
- Nothing is stored anywhere except in the browser during the conversation
- Your API key stays on your machine
- Cost is very small — a typical conversation is a fraction of a cent
