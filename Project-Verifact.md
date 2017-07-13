## Name 

 ⋅⋅⋅Verifact

## Audience

 ⋅⋅⋅Users of internet news sites and aggregators 

## Description

Create a (Chrome and/or Facebook?) plugin that will allow the user to right-click an article headline or right-click from within the article to use the Fact Check or Snopes to verify if the article is legitmate.

## Technologies

Bootstrap/CSS

HTML/5

JavaScript/Jquery

## Creating a Chrome Extension

1. Creating Manifest. JSON:

Every Chrome extension consists of, at minimum, a file called manifest.json, which defines the basics of your extension—its name, description, version number, what kind of extension it is the permissions it needs to run (e.g., what web sites it needs access to), and so on.

2. Content Scripts:

A content script is “a JavaScript file that runs in the context of web pages.” This means that a content script can interact with web pages that the browser visits. To inject the script, we need to tell our manifest.json file about it.

3. Creating UI and implementing the logic:

There are several ways to create UI For your extensions, some of them are Browser Action, Page Action, Developer tools and Omnibox.

4. Load your extension into Chrome/Testing:

To load your extension in Chrome, open up "chrome://extensions/" in your browser and click “Developer mode” in the top right. Now click “Load unpacked extension…” and select the extension’s directory. You should now see your extension in the list.

5. Getting your extension into the Chrome Web Store:

Publish in the Chrome Web Store: https://developer.chrome.com/webstore/publish

Watch the video on how to build chrome extension: https://developer.chrome.com/extensions/getstarted
