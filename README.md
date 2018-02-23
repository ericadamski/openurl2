# opn-url – Node.js module for opening URLs

opn-url is a Node.js module for opening a URL via the operating system. This will usually trigger actions such as:

* http URLs: open the default browser
* mailto URLs: open the default email client
* file URLs: open a window showing the directory (on OS X)

Example interaction on the Node.js REPL:

    > require("openurl").open("http://rauschma.de")
    > require("openurl").open("mailto:john@example.com")

You can generate emails as follows:

    require("openurl").mailto(["john@example.com", "jane@example.com"],
        { subject: "Hello!", body: "This is\nan automatically sent email!\n" });

Install:

    `npm install opn-url`

    or

    `yarn add opn-url`

opn-url:

In the original openurl and the cloned openurl2 package, there was an issue with URL's escaping `&` characters. This has been fixed in this fork. As is seems the original Project, and clone are no longer maintained, we attempted to send in a pull request, with no response we pushed this Fork.
