## Name 

    Verifact

## Audience

    Users of internet news sites and news aggregators as well as social websites.

## Proposal

    Create a Google Chrome plugin that provides users with the capability of comparing
    one article against similar articles found on fact-checking websites. 

## Value Proposition

    With the huge influx in fake news articles onto the internet there is an enormous need
    to provide users with some capability of comparing a suspect article against similar 
    articles culled from fact-checking sources. This plugin isn't meant to replace sites like Snopes 
    or Factcheck.org but rather it complements them by providing the user with a easy, convenient 
    way to judge for themselves the validity of questionable articles. Additionally, this plugin
    also contains a built-in history feature so that users can come back to past searches and
    their results for later referral.

## Technologies

    Bootstrap/CSS
    HTML/5
    JavaScript/Jquery
    Sails (for managing DB API)
    Java for storage and purging of search and historical data
    MySQL (or equivalent RDBMS)

## Product Backlog

    Note: Data will be passed as JSON

    1. View
        a)  Add hook to browser right-click menu to add choice of Verifact
        b)  Create selection submenu below Verifact
            i)  Search For...
            ii) View Usage History
        c)  Create search window and add capability for user to refine search terms
        d)  Create results window
        e)  Create usage history window
            i)      Send a range of dates to pull from
            ii)     Purge usage history based on a range of dates
            iii)    Delete individual history records
        f)  Add search submission
        g)  Add usage history submission
        h)  Add purge usage history submission

    2) Control
        a)  Search
            i)      Receive search requests from View
            ii)     Submit search requests to API(s) & receive results
            iii)    Return search results to View
            iv)     Submit search information and results to DB API for later retrieval

        b)  Usage History
            i)      Receive usage history requests
            ii)     Submit usage history request to DB API
            iii)    Receive usage history results from DB API
            iv)     Return usage history results to View

    3) Model
        a)  Create database for storing usage history
            i)      Date & Time of search request
            ii)     Source URL and search terms of search request
            iii)    List of APIs used for comparators of search request (e.g. Politifact)
            iv)     URL & Title of each search result from search request
        b)  Capability to store received search data for later retrival.
        c)  Capability to purge historical search data by date range or individual record

## Fact-Checking Websites

Politifact: API: http://static.politifact.com/api/v2apidoc.html

Snopes API: Snopes does not appear to have an API

FactCheck: Factcheck.org does not appear to have an API

## Creating a Chrome Extension

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
