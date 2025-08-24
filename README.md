## Introduction to HTML -

- for heading we have html tags from h1 to h6.
- ideally if we use one heading tag in our page then the next subheading in that page should be its child i.e. if we use h1 then subheading should be h2 and not h3 etc..
  - basically the most important thing in the page should be h1, then h2 etc...
- in case we want a data to be separated between multiple paragraphs then it should be done via <p></p> tag as putting spaces between paragaphs in html will not create multiple paras.
- we do not add any data between the tags in void html elements e.g. <hr/>.
  - similarly break element <br/> , it is used to break content into separate lines (while they are still part of same paragraph e.g. poem) in order to have correct meaning.
- tags for unordered and ordered list <ul> or <ol>, themselves do not contain the content but have sub-elements listitems i.e. <li> that contain the actual items of the list.
- <a> tag needs an attribute `href` in order to function correctly like a hyperlink.
- similar to anchor tag <img> tag has a main attribute source or `src` which tells the image element the actual source of the image.

  - we should also always add `alt` attribute to image which means alternate text description that is used by screen reader to describe the image.

- webhosting is the process of making our website available on the internet so that anyone in the world can access it.
  - to do this we need to put all our files and data it consists of (index.html, assets etc..) on to a web server.
  - web server is a server connected to the internet and stuff we put there will be available on the internet ready serve the files to anyone in the world who want to access it.
  -

## Introduction to CSS -

- 3 ways to add css into a website -

  1. inline - when targeting a single element
  2. internal - targeting a single page
  3. external - using <link rel="stylesheet" href="./styles.css"> in head section

- CSS selectors : attribute selector can be used to select elements with certain attributes or attributes with certain value. e.g. p[draggable] { color : red } Or p[draggable="false"] {}

- CSS colors -

  - we can find all the named colors in mdn docs.
  - we can find more color palettes at colorhunt.co

- Font Properties -

  - font properties are for changing the appearance of the text in our websites.
  - e.g. font-weight, font-size, font-family
  - what exactly is 1px , its around 1/96th of an inch == 0.26mm.
  - another unit that we use commonly other than pixel is point i.e. 1pt == 1/72nd inch == 0/35mm (used in many applications like microsoft word)
  - em (pronounced as just m) is also used where 1em == 100% of parent, basically relative the parent.
  - rem is relative to the root of our file (i.e. html tag), 1rem = 100% of root --- this approach is better as its more consistent way of changing the size across our elements.

  - font-weight - keyword (normal or bold) , relative to parent (lighter or bolder) , number (100-900)
  - font-family determines what we want our text to look like (the typeface).
    - e.g. Helvetica is a mac specific type face and many windows computer might not have it , hence when giving font family we also provide a backup generic fontType e.g. sans-sarif (all edges are at right angles while the serif has some decoration around the edges.).
  - for external fonts we can use fonts.google.com and get the link of the font weight that we want and put that link to the head section of the html and then use that style in our css font-family.
  - for external fonts we can use fonts.google.com and get the link of the font weight that we want and put that link to the head section of the html and then use that style in our css font-family.

- CSS Box model :
  - CSS properties **margin, padding , border** along with width and height form a really important css concept known as the box model.
  - height and width allow us to modify the default size of our html element, we can set it with pixel value like 40px or percentage like 100%.
  - border width is not including height and width i.e. if width of an element is set to 40px and border is 10px wide then border will expand outwards i.e. total width will be 40px+10px
  - we can update of some specific sides using indivisual properties like border-top: 0 to remove the top border and keep all the other border.
  - padding is another property that is mostly seen when we have content such as text.
  - adding padding property will mean it will push border outside, but again width and height of our content box does not change.
  - we want to create artificial boxes to group certain elements so that we can style them together then we use div (content division element).
