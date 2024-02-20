# What is a Web Application

## Web Application Stack

### Understanding Server/Client Terminology

- Client: The client refers to the user's web browser that sends requests to the server and renders the web pages it receives. Examples include Chrome, Firefox, and Safari. Client-side technologies include HTML, CSS, and JavaScript, which run in the browser and determine the look and functionality of web pages.

- Server: The server is a computer or software that responds to the client's requests. It hosts the web application, processes incoming requests, performs actions (like reading from a database), and sends responses back to the client. Server-side technologies include web servers (Apache, Nginx), programming languages (Python, PHP, Ruby), and databases (MySQL, PostgreSQL).

### Key Components of a Web Application Stack

- Web Browser (Client): The interface for users to interact with web applications.
- Web Server: Software that handles HTTP requests and serves web content.
- Database Server: Stores and retrieves data required by the application.
- Application Server: Hosts and runs the backend application logic, interacting with the web server and database server.

## What is a URL

URL (Uniform Resource Locator) is a reference or address used to access resources on the internet. It specifies the location of a resource (such as a web page) on a computer network and how to retrieve it. A URL is the most common type of Uniform Resource Identifier (URI), which can be a page, a document, or an image, among other things. Here's a breakdown of its components and how they function:

### Structure of a URL

A typical URL consists of several parts, each serving a specific purpose. Consider the example URL: <http://www.example.com:80/path/to/myfile.html?key1=value1&key2=value2#SomewhereInTheDocument>

- Scheme: http - Specifies the protocol to be used to access the resource on the Internet. In this case, it's HTTP (Hypertext Transfer Protocol), but it could also be HTTPS, FTP, and so on.

- Host Name: <www.example.com> - The domain name of the server (or the IP address) where the resource is hosted. It indicates where to go to find the resource on the network.

- Port: 80 - (Optional) Specifies the port at which the server is listening for requests. Port 80 is the default for HTTP, so it's often omitted in HTTP URLs.

- Path: /path/to/myfile.html - The specific path to the resource on the server. It's akin to the file path on your computer's file system.

- Query: ?key1=value1&key2=value2 - (Optional) A query string that sends data to the server to be used in the generation of the response. Each key-value pair is separated by an ampersand (&).

- Fragment: #SomewhereInTheDocument - (Optional) A fragment identifier allowing browsers to directly navigate to a specific part of the document (usually indicated by an anchor ID in HTML).

### How URLs Work

- Entering the URL: When you type a URL into your web browser and press Enter, the browser interprets the URL to understand what resource you're requesting and how to retrieve it.

- DNS Lookup: The browser looks up the domain name (e.g., <www.example.com>) in the Domain Name System (DNS) to find the corresponding IP address of the server.

- Server Request: The browser sends a request to the server at the found IP address, using the specified protocol (e.g., HTTP/HTTPS).

- Response: The server processes the request and sends back the requested resource, along with a status code (e.g., 200 OK for success).

- Rendering: The browser renders the resource for the user to view, which could be an HTML page, an image, etc.

- Importance of URLs
  - Navigation: URLs are essential for navigating the web, allowing users to directly access a wide range of resources hosted online.
  - Linking: They enable linking between web resources, which is a fundamental aspect of the web's interconnected nature.
  - Accessibility: Well-structured URLs can improve the accessibility and usability of websites, making it easier for users and search engines to understand the content of a page.
