# HTTP
** Hypertext Transfer Protocol **

This is essentially a set of rules defined to allow interaction between a client (a web browser like Chrome or Firefox) and server. It establishes a set of rules that the client and server must follow so that they can understand each other and pass data back and forth. If you type a URL into your browser, your browser will initiate a TCP connection (TCP explanation coming soon). Once there is a connection with the server, the browser, adhering to the HTTP protocol, will organize the information to send in the form of key-value pairs, called headers, so that the server will understand what is being requested.

* Stateless Protocol
  * Every transaction is independent and unrelated to other transactions. Like flipping a coin, the coin doesn't know what side it landed on during the last flip. 

* Methods - These are HTTP request methods that indicate some type of action to be taken by the server. 
  * GET: used to retrieve data from the server. If you click a link on a page and you are brought to a new page, then you sent a GET request to the server, requesting a specific page, and the server responded with the appropriate HTML that makes up that page. 
  * POST: used to submit information to a server. If you are registering for a website, you aren't requesting information from the server, you are trying to POST you're own information to the server. 
  * PUT: used to replace information already on the server.
  * PATCH: used to modify information already on the server.
  * DELETE: used to delete information from a server.
  * There are more methods but I won't go into those here.

