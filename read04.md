# html (ch 4,15) and JS (ch 3)

The < a> tag indicates where the hyperlink starts and the < /a> tag indicates where it ends. Whatever text gets added inside these tags, will work as a hyperlink. Add the URL for the link in the < a href=” ”>. Just keep in mind that you should use the < a>…< /a> tags inside < body>…< /body> tags.

Ex: < a href="/about/about\*team.htm">team< /a>
\*\*\_On larger websites**\* it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.
Structure The diagram on the right shows the directory structure for a fictional entertainment listings website called ExampleArts. The top-level folder is known as the root folder. (In this example, the root folder is called examplearts.) The root folder contains all of the other files and folders for a website.
Home pages
The main homepage of a site written in HTML (and the home pages of each section in a child folder) is called index.html.
**Absolute Hyperlinks**
Absolute hyperlinks are complete addresses that contain all the elements of a URL. They always start with some version of http:// followed by the domain name (for example, www.designisphilosophy.com) and optionally a page/folder. Absolute hyperlinks are used when linking to pages outside of the current site that have a different domain name.
**Relative Hyperlinks**
Relative hyperlinks are addresses that are relative to the current domain or location. They only contain the name of the target page prefixed with any necessary folder moves (for example, default.html).
**_Same Folder_**
To link to a file in the same folder, just use the file name. (Nothing else is needed.)
**_Child Folder_**
For a child folder, use the name of the child folder, followed by a forward slash, then the file name.
To link to music listings from the homepage:
< a href="music/listings.html">Listings< /a>
**_Grandchild Folder_**
Use the name of the child folder, followed by a forward slash, then the name of the grandchild folder, followed by another forward slash, then the file name.
To link to DVD reviews from the homepage:
< a href="movies/dvd/reviews.html">
Reviews< /a>
**_Parent Folder_**
Use ../ to indicate the folder above the current one, then follow it with the file name.
Ex:
To link to the homepage from the music reviews:
< a href="../index.html">Home< /a>
**_Grand Parent Folder_**
Repeat the ../ to indicate that you want to go up two folders (rather than one), then follow it with the file name.
To link to the homepage from the DVD reviews:
< a href="../../index.html">Home< /a>
**Root-relative Hyperlinks\*\*
Root-relative hyperlinks are a subset of relative hyperlinks in which all the links are assumed to start from the root folder (domain name) of the site. They differ from the relative hyperlinks in that the address is prefixed by a forward slash (for example, /default.html).

### How to create mailto link in HTML

The mailto link is written like regular link with extra parameters inside the href attribute:
< a href="mailto:name@email.com">Link text</ a>
| Parameter            |  Description                     |
|----------------------|----------------------------------|
|mailto:name@email.com | e-mail recipient address         |
|cc=name@email.com     | carbon copy e-mail address       |
|bcc=name@email.com    | blind carbon copy e-mail address |
|subject=subject text  | subject of e-mail                |
|body=body text        | body of e-mail                   |
|?                     | first parameter delimiter        |
|&                     | other parameters delimiter       |
