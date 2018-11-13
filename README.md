# Mobile Web Specialist Certification Course - Keith Plaisance
---
#### _Three Stage Course Material Project - Restaurant Reviews_

## Project Overview: Stage 1

### Specification

For the Stage 1 of the **Restaurant Reviews** project, I incrementally converted a static webpage to a mobile-ready web application. To accomplish this, I added accessibility and converted the design to be responsive on different sized displays and accessible for screen reader use. In addition I added a service worker to begin the process of creating a seamless experience for offline users.

### How do I run the application?

1. After downloading the files to your local computer, navigate to the root directory.

2. In this folder, start up a simple HTTP server to serve up the site files on your local computer. 

This can be done within a terminal. Check the version of Python you have: `python -V`. If you have Python 2.x, spin up the server with `python -m SimpleHTTPServer 8000` (or some other port, if port 8000 is already in use.) For Python 3.x, you can use `python3 -m http.server 8000`. If you don't have Python installed, navigate to Python's [website](https://www.python.org/) to download and install the software.

3. With your server running, visit the site: `http://localhost:8000`

4. This will open the Restaurant Reviews application. If Chrome is the browser that opened up, then press F12 to open the Developer Tools. In the console, you will notice there are 0 errors and the Service Worker has been registered.

## Navigating:

Normally the mouse is used to control the application. However with this site, tabbed functionality has been implemented as well. By pressing tab on the keyboard, the user can navigate through the various parts of the app. The first tabbed link is the home link, then the Filter Results, each of the View Details buttons, and finally the footer. Each element (except the footer) is a hyperlink that will take the user somewhere by pressing the Enter key.

On the restaurant detail page, the same functionality works. You start on the home link, then to the "Home" breadcrumb, to each review and finally to the footer. Both home links are active hyperlinks which can be accessed by pressing the Enter key.

## Caching:

An important component of this project is the ability to cache the pages for offline viewing. This is accomplished by using a Service Worker Javascript file. This file loads all the pages into the user's computer cache. This was tested by taking the site offline and full functionality was restored.
