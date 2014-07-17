# Redirect of Requirement

Redirect of Requirement is a web-hosted, information gathering utility that operates in the realm of social engineering.
It utilizes a small set of phishing techniques along with URL-shortening functionality in order to capture information
about a psuedonymous or anonymous parties who may not be acting as carefully as they should. Like the Room of
Requirement, it's designed to be useful to a restricted set of people and appear ordinary to everyone else.

## So really... what does it do?

It captures browser data, header information and IP of people who use it for you to examine and use at your own
discretion. It does this through simple access logs and URL redirection. This redirection could be simple or more
complex, depending on the redirect used. A simple redirect will map one domain to another using the following scheme:

    http://<subdomain>.<domain1>.<TLD>/<path> -> http://<subdomain>.<domain2>.<TLD>/<path>

A complex map will act as a URL shortener and map a short URL to a saved long URL. These may either use a hash
to determine the shortened asset path, or the mapping may be stored in a database, depending on which redirect system
is used.

While the information gathered may seem relatively harmless (you share this data with every website you visit) it
actually is the starting point for some directed attacks. In typical online interactions, you share this data with
trusted or semi-trusted services, but not frequently with individuals. In certain contexts, it may be possible
to use this information to directly link you to an online alias, psuedonym or anonymous post.

## How does it work?

It quietly acts as an access log for an analyst while they trick their target into clicking a link on a 3rd party
service. It won't make you good at social engineering. It won't make people click your link, and it won't make sure
only your target clicks the link. It just records information about whoever clicks the link and redirects them.
It won't make your redirects valid or even convincing, it will just do what it's told.

## Example Use

* A person posts something on a popular link aggregation site online. 
* As an analyst, you deem this person to be interesting, given what they have posted
* **BUT** the user has posted it under an alias and you have no leads from this alias. :(
* **BUT** you do not have a subpoena to get information about the person from the popular link aggregation site either. :(
* You setup a Redirect of Requirement on the free tier of a popular cloud hosting service
* You configure the Redirect of Requirement to have it redirect its entire path directly to the path of a popular image sharing site that is commonly used on the popular link aggregation site.
* You find a relevant image-based-response on the popular image sharing site
* You substitute your domain for the popular image sharing site's domain and hide the new URL behind markdown link text in your response on the popular link aggregation site.
* You respond to a comment long after most people will read it, knowing that the interesting person will be notified that they have a response
* The person clicks the link and is redirected through the Redirect of Requirement, hopefully not noticing the redirect occurred or that the URL is not where they ended up, but only noticing your image-based-response on the popular image sharing site
* You now have information about your interesting user captured in the Redirect of Requirement logs
