# How The Web Works

## Clients and Servers

- Computers connected to the internet are called *clients and servers*

- Clients are the typical web user's internet-connected devices (for example, your computer connected to your Wi-Fi, or phone connected to your mobile network) and web-accessing software available on those devices (Usually a web browser like Firefox or Chrome).

- Servers are computers that store webpages, sites, or apps. When a client device wants to access a webpage, a copy of the webpage is downloaded from the server onto the client machine to be displayed in the user's web browser.

### Other Parts of the Toolbox

- The client and server listed above doesn't tell the entire story. There are other parts involved.

> Example: Imagine the web is a road. One end of the road is the client, another end is the house, and the on the other end of the road is the server, is a store you want to go into.

In addition to the client & server, we need to say hello to:
- Your internet connection: Allows you to send and receive data on the web. It's like the street between your house and the shop.
- TCP/IP: Transmission Control Protocol and Internet Protocol are communication protocols that define how data should travel across the internet. This is like transport mechanisms that let you place an order, go to the shop, and buy your goods.

> Example: The car or bike (or however else you get around).

- DNS: Domain Name System is like an address book for websites. When you type a web address in your browser, the browser looks at the DNS to find out which server the website lives on, so it can send HTTP messages to the right place.

> Example: It's like looking up the address of the shop so you can access it.

- HTTP: Hypertext Transfer Protocol is an application protocol that defines a language for clients and servers to speak to each other.

> Example: The language you use to order the goods.

- Component files: A website is made up of many files, which are like the different parts of the goods you buy from the shop. These files come in two main types:
- Code files: Websites are built primarily from HTML, CSS, and JavaScript, though you'll meet other technologies later.
- Assets: Collective name for all the other stuff that makes up a website, such as iamges, music, video, Word documents, and PDFs.

## So what happens, exactly?

- When you type a web address into your browser (For analogy that's like walking to the shop):

- The browser goes to the DNS server, and finds the real address of the server that the website lives on (you find the address of the shop).

- The browser sends an HTTP request message to the server, asking it to send a copy of the website to the client (you go to the shop and order your goods). This message, and all other data sent to the client and the server, is sent across your internet connection using TCP/IP.

- If the server approves the client's request, the server sends the client a "200 OK" message, which means "Of course you can look at that website! Here it is!" and then startes sending the website's files to the browser as a series of small chunks called ata packets (The shop gives you your goods, and you bring them back to your house).
  
- The browser assembles the small chunks into a complete web page and displays it to you (the goods arrive at your door — new shiny stuff, awesome!).

# Order in which component files are parsed

- When browsers send requests to servers for HTML files, those HTML files often contain *<link>* elements referencing external CSS stylesheets and *<script>* elements referencing external JavaScript scripts. It is important to know the order in which those files are parsed by the browser as the browser loads the page:

- The browser parses the HTML file first, and that leads to the browser recognizing any <link>-element references to external CSS stylesheets and any <script>-element references to scripts.

- As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from <link> elements, and any JavaScript files it has found from <link> elements, and any JavaScript files has found from <script> elements, and from those, then parses the CSS and JavaScript.

- The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and complies and executes the parsed JavaScript.

- As the browser builds the DOM tree and applies the styles from the CSSOM tree executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

# DNS Explained

- Real web addresses aren't the nice, memorable strings you type into your address bar to find your favorite website. They are special numbers that look like this: *192.0.2.162.*
  
- This is called an IP address, and it represents a unique location on the web. However, it's not very easy to remember, is it? That's why the Domain Name System was invented. This system uses special servers that match up a web address you type into your browser (like "mozilla.org") to the website's real (IP) address.
  
- Websites can be reached directly via their addresses. You can use a DNS lookup tool to find the IP address of a website.

# Packets explained

- Earlier we used the term "Packets" to describe the format in which the data is transferred between the client and the server. *What do we mean here?* Basically, when data is sent across the web, It is sent in thousands of small chunks. There are multiple reasons why data is sent in small packets. They are sometimes dropped or corrupted, and it's easier to replace small chunks when this happens. Additionally, the packets can be routed along different paths, making the exchange faster and allowing many different users to download the same website at the same time. If each website was sent as a single big chunk, only one user could download it at a time, which obviously would make the web very inefficient and not much fun to use.

# First Things first: Planning

- Before doing anything, you need some ideas. What should your website actually do? A website can do basically anything, but, for your first try, you should keep things simple. We'll start by creating a simple webpage with a heading, and image, and a few paragraphs.

- To Begin, you'll need to answer these questions:
- What is your website about? Do you like dogs, New York, or Pac-Man?
- What information are you presenting on the subject? Write a title and a few paragraphs and think of an image you'd like to show on your page.
- What does your website look like, in simple high-level terms? What's the background color? What kind of font is appropriate: formal, cartoony, bold and loud, subtle?

# Sketching out your design
- Next, grab pen and paper and sketch out roughly how you want your site to look. For your first simple webpage, there's not much to sketch out, by you should get in the habit of doing this now. It really helps — you don't have to be Van Gogh!

> Note: Even on real, complex websites, the design teams usually start out with rough sketches on paper and later on build digital mockups using a graphics editor or web technologies. Web teams often include both a graphic designer and a user experience (UX) designer. Graphic designers put together the visuals of the website. UX designers have a somewhat more abstract role in addressing how users will experience and interact with the website.

# Choosing your assets
- At this point, it's good to start putting together the content that will eventually appear on your webpage.

# Text

- You should still have your paragraphs and title from earlier. Keep these close by.

# Theme color

- To choose a color, go to the color picker and find a color you like. When you click on a color, you'll see a strange six-character code like #660066. That's called a *hex code* (short for hexadecimal), and represents your color. Copy the code down somewhere safe for now.

# Images

- To choose an image, go to Google Images and search for something suitable.
  
- When you find the image you want, click on the image to get an enlarged view of it.
  
- Right-click the Image (Crtl + Click on a Mac), choose *Save Image As...*, and choose a safe place to saVe your image. Alternatively, copy the image's web address from your browser's address bar for later use.

> Note that most images on the web including in Google Images, are copyrighted. To reduce your likelihood of violating copyright, you can use Google's license filter. Click on the *Tools* button, then on the resulting *Usage* rights option that appears below. You should choose the option *Creative Commons licenses.*

# Font

- As with images, many fonts are protected by licenses, meaning you cannot freely use them in your site. Google Fonts is a web service owned by Google that provides access to many fonts.
  
- Once you found a font, there are two main ways of using it:
  
- Add a reference in your code to load the font from Google's servers.
- Download the font files to your own system, host the font yourself, and use your hosted your copy in your website's code.

> Alternatively you can use safe web fonts such as Arial, Times New Roman, or Courier New.

# JavaScript Basics

- What is JavaScript?

- A powerful programming language that can add interactivity to a website. it was invented by Brendan Eich.

- versatile and beginner-friendly. With more experience, you'll be able to create games, animated 2D and 3D graphics, comprehensive database-driven apps, and much more!
- 
- Relatively compact, yet very flexible. Developers have written a variety of tools on top of the core JavaScript language, unlocking a vast amount of functionality with minimum effort. These include:

> Browser Application Programming Interfaces (APIs) built into web browsers, providing functionality such as dynamically creating HTML and setting CSS styles; collecting and manipulating a video stream from a user's webcam, or generating 3D graphics and audio samples.

- Third-party APIs that allow developers to incorporate functionality in sites from other content providers, such as Twitter or Facebook.
- 
- Third-party frameworks and libraries that you can apply to HTML to accelerate the work of building sites and applications.

# Variables

- Variables are containers that store values. You start by declaring a variable with the let keyword, followed by the name you give to the variable: let myVariable;

- A semicolon at the end of a line indicates where a statement ends. It is only required when you need to separate statements on a single line. However, some people believe it's good practice to have semicolons at the end of each statement. There are other rules for when you should and shouldn't use semicolons.
  
- You can name a variable nearly anything, but there are some restrictions.
  
- JavaScript is case sensitive. This means *myVariable* is **not the same** as *myvariable*. If you have problems in your code, check the case!

- After declaring a variable, you can give it a value:

- myVariable = "Bob";

- Also, you can do both these operations on the same line:

- let myVariable = "Bob";

- You retrieve the value by calling the variable name:

- myVariable;

- After assigning a value to a variable, you can change it later in the code:

- let myVariable = "Bob";

- myVariable = "Steve";

# Comments

- Comments are snippets of text that can be added along with code. The browser ignores text marked as comments. You can write comments in JavaScript just as you can in CSS.

# Answers

In the vast digital space, where data roams,
lies a story of HTTP, sending itself to computer domes.
A language, a protocol, speaking in bytes and code,
Across the web, it's journey unfolds.

It starts with a request, a whisper in the air,
A client speaks softly, with intent and care.
Through cables and routers, it beings its flight,
Seeking a server in the endless night.

Through nodes and switches, it finds its way,
Each hop a dance, a ballet of delay.
Across the networks, it travels far and wide,
Invisible threads in the digital tide.

With headers and payloads, it carries its load,
Through firewalls and gateways, along the road.
Past fire and storm, it perseveres,
In the realm of bits, where everything adheres.

And when it reaches its destination, at long last,
A server responds, the die is cast.
With data in hand, it retraces its track,
Back to the client, no turning back.

Through cyberspace, this dance goes on,
A symphony of packets until dawn.
HTTP, the messenger, the conduit of our age,
In the network's embrace, it writes its page.


- The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and complies and executes the parsed JavaScript.

- Go to Google Images and search for something suitable.

- To create a string in JavaScript, you can use single, double, or backtick quotes. To create a number in JavaScript, you type a number without any quotes surrounding them.

- A variable is a container that store values, they are important because they hold the values necessary for the JavaScript code.

# HTML

- HTML (HyperText Markup Language) is a markup language that tells web browsers how to structure the web pages you visit. It can be as complicated or as simple as the web developer wants it to be. HTML consists of a series of elements, which you use to enclose, wrap, or mark up different parts of content to make it appear or act in a certain way. The enclosing tags can make content into a hyperlink to connect to another page, italicize words, and so on. For example, consider the following line of text:

> My cat is very grumpy

- If we wanted the text to stand by itself, we could specify that it is a paragraph by enclosing it in a paragraph (<p>) element:

> <p>My cat is very grumpy</p>

> Note: Tags in HTML are not case-sensitive. This means they can be written in uppercase or lowercase. For example, a <title> tag could be written as <title>, <TITLE>, <Title>, <TiTlE>, etc., and it will work. However, it is best practice to write all tags in lowercase for consistency and readability.

# Anatomy of an HTML element

- The anatomy of our element is:
  
- The opening tag: This consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets. This opening tag marks where the element begins or starts to take effect. In this example, it precedes the start of the paragraph text.
  
- The content: This is the content of the element. In this example, it is the paragraph text.
  
- The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This marks where the element ends. Failing to include a closing tag is a common beginner error that can produce peculiar results.

> The element is the opening tag, followed by content, followed by the closing tag.

# Nesting elements

- Elements can be placed within other elements. This is called nesting. If we wanted to state that our cat is very grumpy, we could wrap the word very in a <strong> element, which means that the word is to have strong(er) text formatting:

> <p>My cat is <strong>very</strong> grumpy.</p>

- There is a right and wrong way to do nesting. In the example above, we opened the p element first, then opened the strong element. For proper nesting, we should close the strong element first, before closing the p.

- The following is an example of the wrong way to do nesting:

> <p>My cat is <strong>very grumpy.</p></strong>

- The tags have to open and close in a way that they are inside or outside one another. With the kind of overlap in the example above, the browser has to guess at your intent. This kind of guessing can result in unexpected results.

# Void elements

- Not all elements follow the pattern of an opening tag, content, and a closing tag. Some elements consist of a single tag, which is typically used to insert/embed something in the document. Such elements are called void elements. For example, the <img> element embeds an image file onto a page.

> Note: In HTML, there is no requirement to add a / at the end of a void element's tag, for example: <img src="images/cat.jpg" alt="cat" />. However, it is also a valid syntax, and you may do this when you want your HTML to be valid XML.

# Attributes

- Elements can also have attributes. Attributes look like this:

<p class="editor-note">My cat is very grumpy</p>

- Attributes contain extra information about the element that won't appear in the content. In this example, the class attribute is an identifying name used to target the element with style information.

- An attribute should have:
  
- A space between it and the element name. (For an element with more than one attribute, the attributes should be separated by spaces too.)
  
- The attribute name, followed by an equal sign.

- An attribute value, wrapped with opening and closing quote marks.
  
- Active learning: Adding attributes to an element

- The <img> element can take a number of attributes, including:
  
- src: The src attribute is a required attribute that specifies the location of the image. For example: src="https://raw.githubusercontent.com/mdn/beginner-html-site/gh-pages/images/firefox-icon.png".
  
- alt: The alt attribute specifies a text description of the image. For example: alt="The Firefox icon".
  
- width: The width attribute specifies the width of the image with the unit being pixels. For example: width="300".
  
- height: The height attribute specifies the height of the image with the unit being pixels. For example: height="300".
  
# Boolean attributes

- Sometimes you will see attributes written without values. This is entirely acceptable. These are called Boolean attributes. Boolean attributes can only have one value, which is generally the same as the attribute name. For example, consider the disabled attribute, which you can assign to form input elements. (You use this to disable the form input elements so the user can't make entries. The disabled elements typically have a grayed-out appearance.) For example:

> <input type="text" disabled="disabled" />

# Omitting quotes around attribute values

- If you look at code for a lot of other sites, you might come across a number of strange markup styles, including attribute values without quotes. This is permitted in certain circumstances, but it can also break your markup in other circumstances. The element in the code snippet below, <a>, is called an anchor. Anchors enclose text and turn them into links. The href attribute specifies the web address the link points to. You can write this basic version below with only the href attribute, like this:

> <a href=https://www.mozilla.org/>favorite website</a>

- Anchors can also have a title attribute, a description of the linked page. However, as soon as we add the title in the same fashion as the href attribute there are problems:

> <a href=https://www.mozilla.org/ title=The Mozilla homepage>favorite website</a>

- As written above, the browser misinterprets the markup, mistaking the title attribute for three attributes: a title attribute with the value The, and two Boolean attributes, Mozilla and homepage. Obviously, this is not intended! It will cause errors or unexpected behavior, as you can see in the live example below.
> Always include the attribute quotes. It avoids such problems, and results in more readable code.

# Single or double quotes?
- You will also notice that the attributes are wrapped in double quotes. However, you might see single quotes in some HTML code. This is a matter of style. You can feel free to choose which one you prefer. Both of these lines are equivalent:

- <a href='https://www.example.com'>A link to my example.</a>
- <a href="https://www.example.com">A link to my example.</a>

- Make sure you don't mix single quotes and double quotes. This example (below) shows a kind of mixing of quotes that will go wrong:

> <a href="https://www.example.com'>A link to my example.</a>

- However, if you use one type of quote, you can include the other type of quote inside your attribute values:

> <a href="https://www.example.com" title="Isn't this fun?">
  A link to my example.
</a>

- To use quote marks inside other quote marks of the same type (single quote or double quote), use HTML entities. For example, this will break:

<a href="https://www.example.com" title="An "interesting" reference">A link to my example.</a>

- Instead, you need to do this:

- <a href="https://www.example.com" title="An &quot;interesting&quot; reference">A link to my example.</a>

# Anatomy of an HTML document

- Individual HTML elements aren't very useful on their own. Next, let's examine how individual elements combine to form an entire HTML page:
- 
<!doctype html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <title>My test page</title>
  </head>
  <body>
    <p>This is my page</p>
  </body>
</html>

- Here we have:
- <!DOCTYPE html>: The doctype. When HTML was young (1991-1992), doctypes were meant to act as links to a set of rules that the HTML page had to follow to be considered good HTML. Doctypes used to look something like this:
> <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">

- More recently, the doctype is a historical artifact that needs to be included for everything else to work right. <!DOCTYPE html> is the shortest string of characters that counts as a valid doctype. That is all you need to know!

- <html></html>: The <html> element. This element wraps all the content on the page. It is sometimes known as the root element.

- <head></head>: The <head> element. This element acts as a container for everything you want to include on the HTML page, that isn't the content the page will show to viewers. This includes keywords and a page description that would appear in search results, CSS to style content, character set declarations, and more. You will learn more about this in the next article of the series.

- <meta charset="utf-8">: The <meta> element. This element represents metadata that cannot be represented by other HTML meta-related elements, like <base>, <link>, <script>, <style> or <title>. The charset attribute specifies the character encoding for your document as UTF-8, which includes most characters from the vast majority of human written languages. With this setting, the page can now handle any textual content it might contain. There is no reason not to set this, and it can help avoid some problems later.
  
- <title></title>: The <title> element. This sets the title of the page, which is the title that appears in the browser tab the page is loaded in. The page title is also used to describe the page when it is bookmarked.

- <body></body>: The <body> element. This contains all the content that displays on the page, including text, images, videos, games, playable audio tracks, or whatever else.

# Basic sections of a document

- Webpages can and will look pretty different from one another, but they all tend to share similar standard components, unless the page is displaying a fullscreen video or game, is part of some kind of art project, or is just badly structured:
  
- header: Usually a big strip across the top with a big heading, logo, and perhaps a tagline. This usually stays the same from one webpage to another.
  
- navigation bar: Links to the site's main sections; usually represented by menu buttons, links, or tabs. Like the header, this content usually remains consistent from one webpage to another — having inconsistent navigation on your website will just lead to confused, frustrated users. Many web designers consider the navigation bar to be part of the header rather than an individual component, but that's not a requirement; in fact, some also argue that having the two separate is better for accessibility, as screen readers can read the two features better if they are separate.

- main content: A big area in the center that contains most of the unique content of a given webpage, for example, the video you want to watch, or the main story you're reading, or the map you want to view, or the news headlines, etc. This is the one part of the website that definitely will vary from page to page!

- sidebar: Some peripheral info, links, quotes, ads, etc. Usually, this is contextual to what is contained in the main content (for example on a news article page, the sidebar might contain the author's bio, or links to related articles) but there are also cases where you'll find some recurring elements like a secondary navigation system.
- footer:
  
- A strip across the bottom of the page that generally contains fine print, copyright notices, or contact info. It's a place to put common information (like the header) but usually, that information is not critical or secondary to the website itself. The footer is also sometimes used for SEO purposes, by providing links for quick access to popular content.

> Note: The image above illustrates the main sections of a document, which you can define with HTML. However, the appearance of the page shown here - including the layout, colors, and fonts - is achieved by applying CSS to the HTML.

> In this module we're not teaching CSS, but once you have an understanding of the basics of HTML, try diving into our CSS first steps module to start learning how to style your site.

# HTML for structuring content
> Note: Roughly 8% of men and 0.5% of women are colorblind; or, to put it another way, approximately 1 in every 12 men and 1 in every 200 women. Blind and visually impaired people represent roughly 4-5% of the world population (in 2015 there were 940 million people with some degree of vision loss, while the total population was around 7.5 billion).

- In your HTML code, you can mark up sections of content based on their functionality — you can use elements that represent the sections of content described above unambiguously, and assistive technologies like screen readers can recognize those elements and help with tasks like "find the main navigation", or "find the main content." As we mentioned earlier in the course, there are a number of consequences of not using the right element structure and semantics for the right job.
  
- To implement such semantic mark up, HTML provides dedicated tags that you can use to represent such sections, for example:
  
- header: <header>.
  
- navigation bar: <nav>.
  
- main content: <main>, with various content subsections represented by <article>, <section>, and <div> elements.
  
- sidebar: <aside>; often placed inside <main>.
  
- footer: <footer>.

# HTML layout elements in more detail

- <main> is for content unique to this page. Use <main> only once per page, and put it directly inside <body>. Ideally this shouldn't be nested within other elements.

- <article> encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post).

- <section> is similar to <article>, but it is more for grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. It's considered best practice to begin each section with a heading; also note that you can break <article>s up into different <section>s, or <section>s up into different <article>s, depending on the context.

- <aside> contains content that is not directly related to the main content but can provide additional information indirectly related to it (glossary entries, author biography, related links, etc.).

- <header> represents a group of introductory content. If it is a child of <body> it defines the global header of a webpage, but if it's a child of an <article> or <section> it defines a specific header for that section (try not to confuse this with titles and headings).

- <nav> contains the main navigation functionality for the page. Secondary links, etc., would not go in the navigation.

- <footer> represents a group of end content for a page.

# Non-semantic wrappers

- Sometimes you'll come across a situation where you can't find an ideal semantic element to group some items together or wrap some content. Sometimes you might want to just group a set of elements together to affect them all as a single entity with some CSS or JavaScript. For cases like these, HTML provides the <div> and <span> elements. You should use these preferably with a suitable class attribute, to provide some kind of label for them so they can be easily targeted.

<span> is an inline non-semantic element, which you should only use if you can't think of a better semantic text element to wrap your content, or don't want to add any specific meaning. For example:

<p>
  The King walked drunkenly back to his room at 01:00, the beer doing nothing to
  aid him as he staggered through the door.
  <span class="editor-note">
    [Editor's note: At this point in the play, the lights should be down low].
  </span>
</p>

- <div> is a block level non-semantic element, which you should only use if you can't think of a better semantic block element to use, or don't want to add any specific meaning. For example, imagine a shopping cart widget that you could choose to pull up at any point during your time on an e-commerce site:

<div class="shopping-cart">
  <h2>Shopping cart</h2>
  <ul>
    <li>
      <p>
        <a href=""><strong>Silver earrings</strong></a>: $99.95.
      </p>
      <img src="../products/3333-0985/thumb.png" alt="Silver earrings" />
    </li>
    <li>…</li>
  </ul>
  <p>Total cost: $237.89</p>
</div>

- This isn't really an <aside>, as it doesn't necessarily relate to the main content of the page (you want it viewable from anywhere). It doesn't even particularly warrant using a <section>, as it isn't part of the main content of the page. So a <div> is fine in this case. We've included a heading as a signpost to aid screen reader users in finding it.

> Warning: Divs are so convenient to use that it's easy to use them too much. As they carry no semantic value, they just clutter your HTML code. Take care to use them only when there is no better semantic solution and try to reduce their usage to the minimum otherwise you'll have a hard time updating and maintaining your documents.

# Line breaks and horizontal rules:

- Two elements that you'll use occasionally and will want to know about are <br> and <hr>.

- <br>: the line break element

- <br> creates a line break in a paragraph; it is the only way to force a rigid structure in a situation where you want a series of fixed short lines, such as in a postal address or a poem. For example:

<p>
  There once was a man named O'Dell<br />
  Who loved to write HTML<br />
  But his structure was bad, his semantics were sad<br />
  and his markup didn't read very well.
</p>

- Without the <br> elements, the paragraph would just be rendered in one long line.

- <hr>: the thematic break element
- <hr> elements create a horizontal rule in the document that denotes a thematic change in the text (such as a change in topic or scene). Visually it just looks like a horizontal line. As an example:

<p>
  Ron was backed into a corner by the marauding netherbeasts. Scared, but
  determined to protect his friends, he raised his wand and prepared to do
  battle, hoping that his distress call had made it through.
</p>
<hr />
<p>
  Meanwhile, Harry was sitting at home, staring at his royalty statement and
  pondering when the next spin off series would come out, when an enchanted
  distress letter flew through his window and landed in his lap. He read it
  hazily and sighed; "better get back to work then", he mused.
</p>

# What is the HTML head?
- The HTML head is the contents of the <head> element. Unlike the contents of the <body> element (which are displayed on the page when loaded in a browser), the head's content is not displayed on the page. Instead, the head's job is to contain metadata about the document.

# Adding a title

- We've already seen the <title> element in action — this can be used to add a title to the document. This however can get confused with the h1 element, which is used to add a top level heading to your body content — this is also sometimes referred to as the page title. But they are different things!
  
- The h1 element appears on the page when loaded in the browser — generally this should be used once per page, to mark up the title of your page content (the story title, or news headline, or whatever is appropriate to your usage.)

- The <title> element is metadata that represents the title of the overall HTML document (not the document's content.)
  
- The <title> element contents are also used in other ways. For example, if you try bookmarking the page (Bookmarks > Bookmark This Page or the star icon in the URL bar in Firefox), you will see the <title> contents filled in as the suggested bookmark name.
  
- The <title> contents are also used in search results, as you'll see below.

# Metadata
- Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document — the <meta> element. Of course, the other stuff we are talking about in this article could also be thought of as metadata too. There are a lot of different types of <meta> elements that can be included in your page's <head>, but we won't try to explain them all at this stage, as it would just get too confusing.

- In the example we saw above, this line was included:

> <meta charset="utf-8" />

- This element specifies the document's character encoding — the character set that the document is permitted to use. utf-8 is a universal character set that includes pretty much any character from any human language.

> Note: Some browsers (like Chrome) automatically fix incorrect encodings, so depending on what browser you use, you may not see this problem. You should still set an encoding of utf-8 on your page anyway to avoid any potential problems in other browsers.

# Adding an author and description
- Many <meta> elements include name and content attributes:

- `name` specifies the type of meta element it is; what type of information it contains.
- `content` specifies the actual meta content.

- Two such meta elements that are useful to include on your page define the author of the page, and provide a concise description of the page.

> EX: <meta name="author" content="Chris Mills" />
<meta
  name="description"
  content="The MDN Web Docs Learning Area aims to provide
complete beginners to the Web with all they need to know to get
started with developing websites and applications." />

- Specifying an author is beneficial in many ways: it is useful to be able to understand who wrote the page, if you have any questions about the content and you would like to contact them. Some content management systems have facilities to automatically extract page author information and make it available for such purposes.

- Specifying a description that includes keywords relating to the content of your page is useful as it has the potential to make your page appear higher in relevant searches performed in search engines (such activities are termed Search Engine Optimization, or SEO.)

> Note: In Google, you will see some relevant subpages of MDN Web Docs listed below the main homepage link — these are called sitelinks, and are configurable in Google's webmaster tools — a way to make your site's search results better in the Google search engine.

> Note: Many <meta> features just aren't used anymore. For example, the keyword <meta> element (<meta name="keywords" content="fill, in, your, keywords, here">) — which is supposed to provide keywords for search engines to determine relevance of that page for different search terms — is ignored by search engines, because spammers were just filling the keyword list with hundreds of keywords, biasing results.

- As you travel around the web, you'll find other types of metadata, too. A lot of the features you'll see on websites are proprietary creations, designed to provide certain sites (such as social networking sites) with specific pieces of information they can use.

# Adding custom icons to your site

- To further enrich your site design, you can add references to custom icons in your metadata, and these will be displayed in certain contexts. The most commonly used of these is the favicon (short for "favorites icon", referring to its use in the "favorites" or "bookmarks" lists in browsers).

- The humble favicon has been around for many years. It is the first icon of this type: a 16-pixel square icon used in multiple places. You may see (depending on the browser) favicons displayed in the browser tab containing each open page, and next to bookmarked pages in the bookmarks panel.

- A favicon can be added to your page by:

- Saving it in the same directory as the site's index page, saved in .ico format (most also support favicons in more common formats like .gif or .png)
- Adding the following line into your HTML's <head> block to reference it:
- <link rel="icon" href="favicon.ico" type="image/x-icon" />

> Note: If your site uses a Content Security Policy (CSP) to enhance its security, the policy applies to the favicon. If you encounter problems with the favicon not loading, verify that the Content-Security-Policy header's img-src directive is not preventing access to it.

### Answers
- An HTML attribute is the information inside the opening tag.
- The anatomy of an HTML document includes an opening tag, the content inside of the opening and closing tags (<p>), attribute (a href), empty elements (<br>), and nesting elements.
- Article and section elements in HTML are used to structure and organize content, but they have different purposes. Article element is used for an independent piece of content that could be reused. Section element is used for grouping content within a document.
- A typical website includes the following elements: </!DOCTYPE html>, </html>, </head>, </body>, </headings>, </paragraphs>, </images>, </links>, </lists>.
- Metadata influences the SEO by providing information about a webpage to the search engines.
- The </Meta> tag is used to to find metadata, which provides information about the document.

## Things I want to know more about
- Metadata and how it works?
- Metadata and how it plays a role in SEO?
- API's
