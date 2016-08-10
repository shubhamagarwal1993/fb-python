# Simple Facebook Messenger
This will run on local computer, not hosted yet

Writting in python (flask)

## Run this everytime to run bot
* python `server.py`

### Original steps to set up basic app which replies
* Code:
    * `pip install Flask`
    * See `original_code.py` for what all we need to set up basic communication
    * `ngrok http 5000`. This will give us a link on which facebook messenger can talk to us.
      * Will have to install ngrok
      * This ngrok command may be outdated, see the latest way of writing it
      * ngrok address should look similar to `https://ac433506.ngrok.io`.
    * Go to webhook settings in facebook, and paste above address in the Webhook setup popup.
    * Check mark all the things interested in. I check marked all
    * Also add the verify token
    * If verified successfully, the popup closes and you can now click `subscribe`.
  * Remember to have the correct `ACCESS_TOKEN` in your code.
* Now send a message on messenger and see the reverse of your string being replied.

### Original steps to setup
* Make facebook page and app
* Make a webhook and callback URL
    * Add messenger as a product on fb page settings
    * Name a verification token (I named it `secret`)
    * Generate `Page Access Token` in the messenger tab in settings
    * Go to the webhooks section
    * 
