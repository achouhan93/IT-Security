IT-Security Assignment 3:

In this repository as a part of IT-Security Module Assignment, at the first commit a Web Page is created which is deliberately Vulnerable to Cross Site Scripting.

a) First commit consist of document.write() for the search input field which helps to display the content on the web page.
	Vulnerability: document.write() allows execution of code between <script> tag and also for all HTML tags like <b> tag or <u> tag. 
	Solution	 : document.write() is replaced with document.innerHTML().

b) Second commit consist of document.innerHTML() instead of document.write() for the search field which helps to display the content on the web page.
   Also innerHTML() does not allow the code between <script> tag to be executed.
	Vulnerability: document.innerHTML() allows execution of code in <img> tag.
	Solution	 : document.innerHTML() is then replaced with document.textcontent().

c) Third commit consist of document.textcontent() instead of document.innerHTML() for the search field which helps to disply the content on the web page.
   And document.textcontent() consider the text inserted into the input field as text irrespective of html tags. 
