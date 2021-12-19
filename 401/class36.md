# Class 36 Reading

---

**What are the advantages of storing tokens in “Cookies” vs “Local Storage”**

- An XSS attack happens when “malicious” JavaScript is injected into a website. Some ways in which this code injection can happen are incorrect input / output validation, a rogue third party script being loaded into the site’s frontend code or social engineering.

- If using localstorage, the malicious JS code can easily read the session tokens and transmit them to the attacker. The attacker would then put these tokens into their browser and have significant, if not complete access to that user’s account.

- Cookies have this special flag called httpOnly. If set, it prevents any JS on the frontend from reading that cookie’s value. This means that the malicious JS code cannot send the access token to the attacker. However, that code can still do malicious API calls while the user is using the site. Depending on the product and the reason for the attack, that may not be enough to fulfill the attacker’s intention.

**Explain 3rd party cookies**

Third-party cookies are created by domains that are not the website (or domain) that you are visiting. These are usually used for online-advertising purposes and placed on a website through adding scripts or tags. A third-party cookie is accessible on any website that loads the third-party server’s code.

Online advertising is the most common use of third-party cookies. By adding their tags to a page, which may or may not display adverts, advertisers can track a user (or their device) across many of the websites they visit.

**How do pixel tags work?**

The website operator or sender of an email adds the tracking pixel using a code in the website’s HTML code or email. This code contains an external link to the pixel server. If a user visits the destination website, the HTML code is processed by the client – usually the user’s browser. The browser follows the link and opens the (invisible) graphic. This is registered and noted in the server’s log files.

In addition, various information about the user is also transmitted using this method. To some extent, combination with JavaScript is necessary in order to collect information about the operating system or browser type.

---

## Document the following Vocabulary Terms

**cookies**: cookies are small blocks of data created by a web server while a user is browsing a website and placed on the user's computer or other device

**authorization**: the process of giving someone the ability to access a resource.

**access control**: it is a security technique that regulates who or what can view or use resources in a computing environment.

**conditional rendering**: rendering the components based on a condition to be true.
