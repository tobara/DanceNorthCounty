# DanceNorthCounty

Instructions to client.

I have attached a zip file that has all applicable files that are needed in order to load the landing page (welcome.html) in mobile version.  It is my assumption because of the age of the website that there is a very high probability that he is running a static html website (no files change name or location.)  There should be in all likely hood a public folder where he most likely uploads files to, when updating the the website.  The attached files and directories need to be placed in that public folder.

Once this task is completed a small code snippet needs to be added to the current welcome.html file.  I have pasted the code snippet below.  I suggest for the sake of ease, simply placing this snippet right below the <html> tag.  But, prior to the <head> tag.  These should be at the very top of the web page.  Once the snippet is in place and the file is saved. It would need to be uploaded to replace the old welcome.html. This code will make it so, if the available screen width is less than or equal to 800 pixels; an alternate (mobile) html web page will be loaded.  In this case mWelcome.html instead of Welcome.html.  I hope this satisfies his requirements.

You should be able to check to see if it is functional by simply loading the website on a mobile device.  After everything has been uploaded, including the edited welcome.html

Please feel free to reach out to me via email, text, or phone,  if you have any questions.  The other web pages can be completed rather quickly.  However, without direct access to the server, I would rather make sure we have complete functionality, prior to proceeding with the remaining web pages.  Thanks!

<script type="text/javascript">
   var screenSize = window.screen.availWidth;
   if (screenSize <= 800) {
      var path = window.location.pathname;
      var page = path.split("/").pop();
      var loadMobile = ( 'm' + page );

      document.location = loadMobile;
    }
</script>
