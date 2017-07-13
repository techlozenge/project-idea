## Name 

    Verifact

## Audience

    Readers of internet news sites and news aggregators.

## Proposal

    Create an application that will allow the user to select an article headline or from within the
    article to use Politifact, (FactCheck and Snopes optionl)  the user to 

## Value Proposition

    With the huge influx in fake news articles onto the internet there is an enormous need to provide
    users with some capability of comparing a suspect article against similar articles from reputable
    sources of truth. No application can judge whether or not something is true or false. This application
    gives users a convenient way to judge for themselves the validity of questionable articles. 

## Technologies

    Bootstrap/CSS
    HTML/5
    JavaScript/Jquery
    MySQL (or equivalent RDBMS)

## Product Backlog

    1. Frontend
        a) Selection
            i) 
        b) Query
            i)  

    2. 
        a) 

    3. Backend
        a) Database receives article information


## Additional Information

Snopes API: Snopes does not appear to have an API but it is possible to use Google

FactCheck: 

Politifact: API: http://static.politifact.com/api/v2apidoc.html

Creating a Chrome Extension

    1. Creating Manifest. JSON:

        Every Chrome extension consists of, at minimum, a file called manifest.json, which defines
        the basics of your extension—its name, description, version number, what kind of extension it is
        the permissions it needs to run (e.g., what web sites it needs access to), and so on.

    2. Content Scripts:

        A content script is “a JavaScript file that runs in the context of web pages.” This means 
        that a content script can interact with web pages that the browser visits. To inject the 
        script, we need to tell our manifest.json file about it.

    3. Creating UI and implementing the logic:

        There are several ways to create UI For your extensions, some of them are Browser 
        Action, Page Action, Developer tools and Omnibox.

    4. Load your extension into Chrome/Testing:

        To load your extension in Chrome, open up "chrome://extensions/" in your browser 
        and click “Developer mode” in the top right. Now click “Load unpacked extension…” 
        and select the extension’s directory. You should now see your extension in the list.

    5. Getting your extension into the Chrome Web Store:

        Publish in the Chrome Web Store: https://developer.chrome.com/webstore/publish

        Watch the video on how to build chrome extension: https://developer.chrome.com/extensions/getstarted
