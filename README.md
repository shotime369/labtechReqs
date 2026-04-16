## LabTechReqs: School Practical Booking System
How to create a school science practical booking system using Google apps only

### Setup Instructions

1.  Set up a Google Sheet and navigate to `Extensions > Apps Script`. Add the API code required to link the Sheet with your Google Sites calendar.

2.  You need to deploy the script. Copy the URL found under `Deploy > Manage Deployments`.  
    > **warning:** Deployment is kind of a PITA and often this is the part that will go wrong. If the system breaks, double-check that you have the correct version deployed and that the URL matches exactly.
3.  Using notepad or a code editor, replace your URL into the appropriate place in the HTML:
      ```html
    <script src="function loadBookings() {
            buildCalendar(); 
            if (WEB_APP_URL === "YOUR_APPS_SCRIPT_URL_HERE") return;"></script>
    ```
This is where you customise your own calendar here with teachers names, periods, breaks, colours etc.. 
There are many browser based editors, I use https://playcode.io/ to get a live preview.

4.  Copy your final HTML code and paste it into your Google Sites page using `Embed > Embed Code`.

---


