Zip-It! File Zipper – Matt Pass
Version 1.1.0

Introduction
Zip-It! quite simply, is a component that automatically zips up files & folders you’d like, into a zip file.

Upon making a request to add files and folders to a zip, it first of all quickly and intelligently verifies that these files and folders exist. Once done with the verification, it will then create (or overwrite) a zip file and add all of these files, folders (and sub-folders and files recursively within them), into the zip. Upon completion, it can then provide a download link to the user, which when clicked on starts a header based download, so they may begin downloading the zip.

Zip-It! is the perfect solution for packing files on the fly and providing a download option to the user if you wish.

Setup
Installation of Zip-It! couldn’t be simpler;

1. Copy zip-it.php, zip-it-download-zip.php and zip-it.css to your website.
2. Create a new folder, called zips and change the write permissions on this folder to allow the public to write to it (most commonly referred to as changing the CHMOD permissions to allow public write access).
3. Set a HTML form to send form fields to zip-it.php via a POST form sending method, ensuring that the field name begins with _zipIt and the value of that field contains the filename or folder that you wish to include in the zip. Please ensure you end folders with a trailing to indicate it’s a folder and not a file.

Example:
<form action="zip-it.php" method="POST">
<input type="hidden" name="_zipItFile1" value="images/Birds.jpg">
<input type="hidden" name="_zipItFile2" value="images/Castles.jpg">
<input type="hidden" name="_zipItFile3" value="trips/">
<input type=”submit” name=”submit” value=”Zip It!”>
</form>

That’s it! When you click the button, your specified files will be packed up into a zip and a download link provided. Clicking this will then prompt a download in your web browser. Note: Should you run into any problems, please check to ensure you have the php_zip extension enabled.

Making it your own
Obviously this is enough to get things operating but you will likely want to modify Zip-It! to suit your needs.
Some things you may want to consider include;

•	Changing the style/design to fit seamlessly with your website
•	Altering the flow of Zip-It! to fit in with the flow of actions on your website
•	Changing $zipFileName so the zip’s filename is still unique but not just a number
•	Turning on the $overwriteZip parameter so users can overwrite zips they produce
•	Adding an email option, so users can email the zip as an attachment

Hopefully you can see the benefits of zipping files up quickly and easily using Zip-It!

Happy zipping!
