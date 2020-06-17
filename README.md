# pdf-certificate-downlode-Contact-form-Validation-website
Validating a web page is a process of ensuring that it conforms to the norms or standards defined by the World Wide Web Consortium (W3C) which is the authority to maintain HTML standards.

There are several specific reasons for validating a web page, some of them are:

It helps to create web pages that are cross-browser, cross-platform compatible. It also likely to be compatible with the future version of web browsers and web standards.

Standards compliant web pages increase the search engine spiders and crawlers visibility, as a result your web pages will more likely be appear in search results.

It will reduce unexpected errors and make your web pages more accessible to the visitor.
The first thing we will do is to pass all variables through PHP's htmlspecialchars() function.

When we use the htmlspecialchars() function; then if a user tries to submit the following in a text field:

<script>location.href('http://www.hacked.com')</script>

- this would not be executed, because it would be saved as HTML escaped code, like this:

&lt;script&gt;location.href('http://www.hacked.com')&lt;/script&gt;

The code is now safe to be displayed on a page or inside an e-mail.

We will also do two more things when the user submits the form:

Strip unnecessary characters (extra space, tab, newline) from the user input data (with the PHP trim() function)
Remove backslashes (\) from the user input data (with the PHP stripslashes() function)
