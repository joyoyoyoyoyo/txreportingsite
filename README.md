# txreportingsite

There is now a law in effect in Texas where you cannot get an abortion after 6 weeks, and there is a website where you can report doctors performing abortions. I wrote a bot that will fill out the form every minute. It types out the responses slowly and goes to the next text box every few seconds to mimic a human so it passes the Captcha. However, the website has been updated to not show the form to people outside of Texas. I connected to a VPN in Texas, and while it works when I load it in my browser, it won't load in my testing suite, meaning I've been unable to test about half of my code. I thought I would upload it to Github in case anyone is interested in it, and theoretically it should all work, but I can't guarantee it.

<b>Note:</b> you probably need to download the Chromedriver to your computer yourself and then change the file path in your code. You can download the Chromedriver here: https://chromedriver.chromium.org/downloads

<b>Includes: </b>
- Auto-name generation by scraping from a name generation website for the doctor field.
- Auto-location generation via the uszipcode library. Queries for all TX zip codes, randomly selects one, and then gets the city and county from that zipcode to put into the form.
- Human-like entry so it (theoretically) passes the Captcha (I got it to pass once, and then the site stopped working, which is why I'd still say it's theoretical).
- Autorefreshes the page every minute, and runs again until you stop the program.

I am not responsible for any pro-lifers upset by the existence of this program. I'm just putting my computer science degree to good use.
