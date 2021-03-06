# bootstrap

Bootstrap:
----------
Bootstrap is a free front-end framework for faster and easier web development
Bootstrap includes HTML and CSS based design templates for typography, forms, buttons, tables, navigation, modals, image carousels and many other, as well as optional JavaScript plugins
Bootstrap also gives you the ability to easily create responsive designs

Responsive Web Design:
---------------------
Responsive web design is about creating web sites which automatically adjust themselves to look good on all devices, from small phones to large desktops.

Advantages of Bootstrap:
------------------------
Easy to use: Anybody with just basic knowledge of HTML and CSS can start using Bootstrap
Responsive features: Bootstrap's responsive CSS adjusts to phones, tablets, and desktops
Mobile-first approach: In Bootstrap 3, mobile-first styles are part of the core framework
Browser compatibility: Bootstrap is compatible with all modern browsers (Chrome, Firefox, Internet Explorer, Safari, and Opera)

One advantage of using the Bootstrap CDN:
-----------------------------------------
Many users already have downloaded Bootstrap from MaxCDN when visiting another site. As a result, it will be loaded from cache when they visit your site, which leads to faster loading time. Also, most CDN's will make sure that once a user requests a file from it, it will be served from the server closest to them, which also leads to faster loading time.

Bootstrap 3 is mobile-first:
---------------------------
Bootstrap 3 is designed to be responsive to mobile devices. Mobile-first styles are part of the core framework.
To ensure proper rendering and touch zooming, add the following <meta> tag inside the <head> element:
<meta name="viewport" content="width=device-width, initial-scale=1">
The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).
The initial-scale=1 part sets the initial zoom level when the page is first loaded by the browser.

Containers:
----------
Bootstrap also requires a containing element to wrap site contents.
There are two container classes to choose from:
The .container class provides a responsive fixed width container
The .container-fluid class provides a full width container, spanning the entire width of the viewport
Note: Containers are not nestable (you cannot put a container inside another container).

container.html:
---------------
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
</head>
<body>
  
<div class="container">
  <h1>My First Bootstrap Page</h1>
  <p>This part is inside a .container class.</p> 
  <p>The .container class provides a responsive fixed width container.</p>           
</div>

</body>
</html>

container-fluid.html:
---------------------
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
</head>
<body>
  
<div class="container-fluid">
  <h1>My First Bootstrap Page</h1>      
  <p>This part is inside a .container-fluid class.</p> 
  <p>The .container-fluid class provides a full width container, spanning the entire width of the viewport.</p>           
</div>

</body>
</html>

Bootstrap Grid System:
----------------------
Bootstrap's grid system allows up to 12 columns across the page.
If you do not want to use all 12 columns individually, you can group the columns together to create wider columns:

Grid Classes:
-------------
The Bootstrap grid system has four classes:

xs (for phones)
sm (for tablets)
md (for desktops)
lg (for larger desktops)
The classes above can be combined to create more dynamic and flexible layouts.

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
</head>
<body>
  
<div class="container">
  <h1>My First Bootstrap Page</h1>
  <p>This part is inside a .container class.</p> 
  <p>The .container class provides a responsive fixed width container.</p>       
    
    
    
    <br><br>
    <div class="row">
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
    </div>
    <br><br>
    <div class="row">
      <div class="col-md-2">.col-md-2</div>
      <div class="col-md-2">.col-md-2</div>
      <div class="col-md-2">.col-md-2</div>
      <div class="col-md-2">.col-md-2</div>
      <div class="col-md-2">.col-md-2</div>
      <div class="col-md-2">.col-md-2</div>
    </div>
    <br><br>
    <div class="row">
      <div class="col-md-4">.col-md-4</div>
      <div class="col-md-4">.col-md-4</div>
      <div class="col-md-4">.col-md-4</div>
    </div>
     <br><br>
    <div class="row">
      <div class="col-md-6">.col-md-6</div>
      <div class="col-md-6">.col-md-6</div>
    </div>
     <br><br>
    <div class="row">
      <div class="col-md-12">.col-md-12</div>
    </div>
    <h1>Two Unequal Columns</h1>
    <br><br>
    <div class="row">
      <div class="col-sm-4">.col-sm-4</div>
      <div class="col-sm-8">.col-sm-8</div>
    </div>
    
    
    
</div>
    
    
    

</body>
</html>

Bootstrap's Default Settings:
-----------------------------
Bootstrap's global default font-size is 14px, with a line-height of 1.428.
This is applied to the <body> element and all paragraphs (<p>).
In addition, all <p> elements have a bottom margin that equals half their computed line-height (10px by default).

   <br><br>
    <h1>Open Print</h1>
    <div class="container">
      <h1>Keyboard Inputs</h1>
      <p>To indicate input that is typically entered via the keyboard, use the kbd element:</p>
      <p>Use <kbd>ctrl + p</kbd> to open the Print dialog box.</p>
    </div>
    
    <br><br>
    <h1>Bootstrap Text</h1>
    <div class="container">
      <h2>Contextual Colors</h2>
      <p>Use the contextual classes to provide "meaning through colors":</p>
      <p class="text-muted">This text is muted.</p>
      <p class="text-primary">This text is important.</p>
      <p class="text-success">This text indicates success.</p>
      <p class="text-info">This text represents some information.</p>
      <p class="text-warning">This text represents a warning.</p>
      <p class="text-danger">This text represents danger.</p>
    </div>
    
    
    <br><br>
    <h1>Bootstrap Background</h1>
    <div class="container">
      <h2>Contextual Backgrounds</h2>
      <p>Use the contextual background classes to provide "meaning through colors":</p>
      <p class="bg-primary">This text is important.</p>
      <p class="bg-success">This text indicates success.</p>
      <p class="bg-info">This text represents some information.</p>
      <p class="bg-warning">This text represents a warning.</p>
      <p class="bg-danger">This text represents danger.</p>
    </div>
    
    <br><br>
    <h1>Text Align</h1>
    <div class="container">
      <h2>Typography</h2>
      <p class="text-left">Left-aligned text.</p>
      <p class="text-right">Right-aligned text.</p>      
      <p class="text-center">Center-aligned text.</p>
      <p class="text-justify">Justified text. Justified text. Justified text. Justified text. Justified text. Justified text.</p>      
      <p class="text-nowrap">No wrap text. No wrap text. No wrap text. No wrap text.</p>
      <p><strong>Tip:</strong> Try to resize the browser window to see the behaviour of justify and nowrap.</p>      
    </div>
    
     <br><br>
    <h1>Text Case</h1>
    <div class="container">
      <h2>Typography</h2>
      <p class="text-lowercase">Lowercased text.</p>
      <p class="text-uppercase">Uppercased text.</p>      
      <p class="text-capitalize">Capitalized text.</p>
    </div>
    
     <br><br>
     <h1>Scroll</h1>
     <p>If you add the .pre-scrollable class, the pre element gets a max-height of 350px and provides a y-axis scrollbar:</p>
      <pre class="pre-scrollable">Text in a pre element
      is displayed in a fixed-width
      font, and it preserves
      both      spaces and
      line breaks.</pre>


Bootstrap Tables:
-----------------
The .table class adds basic styling to a table:
The .table-striped class adds zebra-stripes to a table:
The .table-bordered class adds borders on all sides of the table and cells:
The .table-hover class adds a hover effect (grey background color) on table rows:
The .table-condensed class makes a table more compact by cutting cell padding in half:
The .table-responsive class creates a responsive table which will scroll horizontally on small devices:

<br><br>
    <h2>Basic Table</h2>
    <h3>The .table class adds basic styling to a table:</h3>
      <p>The .table class adds basic styling (light padding and only horizontal dividers) to a table:</p>            
      <table class="table">
        <thead>
          <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Email</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>John</td>
            <td>Doe</td>
            <td>john@example.com</td>
          </tr>
          <tr>
            <td>Mary</td>
            <td>Moe</td>
            <td>mary@example.com</td>
          </tr>
          <tr>
            <td>July</td>
            <td>Dooley</td>
            <td>july@example.com</td>
          </tr>
        </tbody>
      </table>
    
    <br><br>
    <h2>Striped Rows</h2>
      <p>The .table-striped class adds zebra-stripes to a table:</p>            
      <table class="table table-striped">
        <thead>
          <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Email</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>John</td>
            <td>Doe</td>
            <td>john@example.com</td>
          </tr>
          <tr>
            <td>Mary</td>
            <td>Moe</td>
            <td>mary@example.com</td>
          </tr>
          <tr>
            <td>July</td>
            <td>Dooley</td>
            <td>july@example.com</td>
          </tr>
        </tbody>
      </table>
    
    
     <br><br>
       <h2>Bordered Table</h2>
      <p>The .table-bordered class adds borders to a table:</p>            
      <table class="table table-bordered">
        <thead>
          <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Email</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>John</td>
            <td>Doe</td>
            <td>john@example.com</td>
          </tr>
          <tr>
            <td>Mary</td>
            <td>Moe</td>
            <td>mary@example.com</td>
          </tr>
          <tr>
            <td>July</td>
            <td>Dooley</td>
            <td>july@example.com</td>
          </tr>
        </tbody>
      </table>
    
    <br><br>
    <h2>Hover Rows</h2>
  <p>The .table-hover class enables a hover state on table rows:</p>            
  <table class="table table-hover">
    <thead>
      <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Email</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>John</td>
        <td>Doe</td>
        <td>john@example.com</td>
      </tr>
      <tr>
        <td>Mary</td>
        <td>Moe</td>
        <td>mary@example.com</td>
      </tr>
      <tr>
        <td>July</td>
        <td>Dooley</td>
        <td>july@example.com</td>
      </tr>
    </tbody>
  </table>
    
    <br><br>
     <h2>Condensed Table</h2>
      <p>The .table-condensed class makes a table more compact by cutting cell padding in half:</p>            
      <table class="table table-condensed">
        <thead>
          <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Email</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>John</td>
            <td>Doe</td>
            <td>john@example.com</td>
          </tr>
          <tr>
            <td>Mary</td>
            <td>Moe</td>
            <td>mary@example.com</td>
          </tr>
          <tr>
            <td>July</td>
            <td>Dooley</td>
            <td>july@example.com</td>
          </tr>
        </tbody>
      </table>
    
    <br><br>
    <h2>Contextual Classes</h2>
      <p>Contextual classes can be used to color table rows or table cells. The classes that can be used are: .active, .success, .info, .warning, and .danger.</p>
      <table class="table">
        <thead>
          <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Email</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Default</td>
            <td>Defaultson</td>
            <td>def@somemail.com</td>
          </tr>      
          <tr class="success">
            <td>Success</td>
            <td>Doe</td>
            <td>john@example.com</td>
          </tr>
          <tr class="danger">
            <td>Danger</td>
            <td>Moe</td>
            <td>mary@example.com</td>
          </tr>
          <tr class="info">
            <td>Info</td>
            <td>Dooley</td>
            <td>july@example.com</td>
          </tr>
          <tr class="warning">
            <td>Warning</td>
            <td>Refs</td>
            <td>bo@example.com</td>
          </tr>
          <tr class="active">
            <td>Active</td>
            <td>Activeson</td>
            <td>act@example.com</td>
          </tr>
        </tbody>
      </table>

    <br><br>
     <h2>Table</h2>
      <p>The .table-responsive class creates a responsive table which will scroll horizontally on small devices (under 768px). When viewing on anything larger than 768px wide, there is no difference:</p>                                                                                      
      <div class="table-responsive">          
      <table class="table">
        <thead>
          <tr>
            <th>#</th>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
            <th>City</th>
            <th>Country</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1</td>
            <td>Anna</td>
            <td>Pitt</td>
            <td>35</td>
            <td>New York</td>
            <td>USA</td>
          </tr>
        </tbody>
      </table>



Bootstrap Images:
-----------------
Rounded Corners
The .img-rounded class adds rounded corners to an image (IE8 does not support rounded corners):

    <br><br>
    <h2>Rounded Corners</h2>
      <p>The .img-rounded class adds rounded corners to an image (not available in IE8):</p>            
      <img src="Koala.jpg" class="img-rounded" alt="Cinque Terre" width="304" height="236"> 
       
    <br><br>
    <h2>Circle</h2>
      <p>The .img-circle class shapes the image to a circle (not available in IE8):</p>            
      <img src="Koala.jpg" class="img-circle" alt="Cinque Terre" width="304" height="236"> 
    
    <br><br>
    <h2>Thumbnail</h2>
      <p>The .img-thumbnail class creates a thumbnail of the image:</p>            
      <img src="Koala.jpg" class="img-thumbnail" alt="Cinque Terre" width="304" height="236">   
          
    <br><br>
     <h2>Image</h2>
      <p>The .img-responsive class makes the image scale nicely to the parent element (resize the browser window to see the effect):</p>
      <img class="img-responsive" src="Koala.jpg" alt="Chania" width="460" height="345"> 
          
    <br><br>
    <h2>Image Gallery</h2>
      <p>The .thumbnail class can be used to display an image gallery.</p>
      <p>The .caption class adds proper padding and a dark grey color to text inside thumbnails.</p>
      <p>Click on the images to enlarge them.</p>
      <div class="row">
        <div class="col-md-4">
          <div class="thumbnail">
            <a href="Koala.jpg" target="_blank">
              <img src="Koala.jpg" alt="Lights" style="width:100%">
              <div class="caption">
                <p>Lorem ipsum donec id elit non mi porta gravida at eget metus.</p>
              </div>
            </a>
          </div>
        </div>
        <div class="col-md-4">
          <div class="thumbnail">
            <a href="Koala.jpg" target="_blank">
              <img src="Koala.jpg" alt="Nature" style="width:100%">
              <div class="caption">
                <p>Lorem ipsum donec id elit non mi porta gravida at eget metus.</p>
              </div>
            </a>
          </div>
        </div>
        <div class="col-md-4">
          <div class="thumbnail">
            <a href="Koala.jpg" target="_blank">
              <img src="Koala.jpg" alt="Fjords" style="width:100%">
              <div class="caption">
                <p>Lorem ipsum donec id elit non mi porta gravida at eget metus.</p>
              </div>
            </a>
          </div>
        </div>
      </div>
          
    <br><br>
    <h2>Responsive Embed</h2>
      <p>Create a responsive video and scale it nicely to the parent element with an 16:9 aspect ratio</p>
      <div class="embed-responsive embed-responsive-16by9">
        <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/XGSy3_Czz8k"></iframe>
      </div>


Bootstrap Jumbotron and Page Header:
------------------------------------
Creating a Jumbotron:
A jumbotron indicates a big box for calling extra attention to some special content or information.
A jumbotron is displayed as a grey box with rounded corners. It also enlarges the font sizes of the text inside it.
Tip: Inside a jumbotron you can put nearly any valid HTML, including other Bootstrap elements/classes.
Use a <div> element with class .jumbotron to create a jumbotron:

Creating a Page Header
A page header is like a section divider.
The .page-header class adds a horizontal line under the heading (+ adds some extra space around the element):

<br><br>
    <div class="jumbotron">
    <h1>Bootstrap Tutorial</h1>      
    <p>Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile-first projects on the web.</p>
      </div>
      <p>This is some text.</p>      
      <p>This is another text.</p>      
    </div>


    <br><br>
     <div class="page-header">
    <h1>Example Page Header</h1>      
      </div>
      <p>This is some text.</p>      
      <p>This is another text.</p> 

Bootstrap Wells:
----------------
The .well class adds a rounded border around an element with a gray background color and some padding:

<br><br>
    <h2>Well</h2>
      <div class="well">Basic Well</div>
      <div class="well well-sm">Small Well</div>
      <div class="well">Normal Well</div>
      <div class="well well-lg">Large Well</div>

Bootstrap Alerts:
-----------------
Bootstrap provides an easy way to create predefined alert messages:

<br><br>
     <h2>Alerts</h2>
      <div class="alert alert-success">
        <strong>Success!</strong> This alert box could indicate a successful or positive action.
      </div>
      <div class="alert alert-info">
        <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
      </div>
      <div class="alert alert-warning">
        <strong>Warning!</strong> This alert box could indicate a warning that might need attention.
      </div>
      <div class="alert alert-danger">
        <strong>Danger!</strong> This alert box could indicate a dangerous or potentially negative action.
      </div>
    
    <br><br>
    <h2>Alert Links</h2>
      <p>Add the alert-link class to any links inside the alert box to create "matching colored links".</p>
      <div class="alert alert-success">
        <strong>Success!</strong> You should <a href="#" class="alert-link">read this message</a>.
      </div>
      <div class="alert alert-info">
        <strong>Info!</strong> You should <a href="#" class="alert-link">read this message</a>.
      </div>
      <div class="alert alert-warning">
        <strong>Warning!</strong> You should <a href="#" class="alert-link">read this message</a>.
      </div>
      <div class="alert alert-danger">
        <strong>Danger!</strong> You should <a href="#" class="alert-link">read this message</a>.
      </div>
    
      <br><br>
      <h2>Alerts</h2>
      <p>The a element with class="close" and data-dismiss="alert" is used to close the alert box.</p>
      <p>The alert-dismissible class adds some extra padding to the close button.</p>
      <div class="alert alert-success alert-dismissable">
        <a href="#" class="close" data-dismiss="alert" aria-label="close">×</a>
        <strong>Success!</strong> This alert box could indicate a successful or positive action.
      </div>
      <div class="alert alert-info alert-dismissable">
        <a href="#" class="close" data-dismiss="alert" aria-label="close">×</a>
        <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
      </div>
      <div class="alert alert-warning alert-dismissable">
        <a href="#" class="close" data-dismiss="alert" aria-label="close">×</a>
        <strong>Warning!</strong> This alert box could indicate a warning that might need attention.
      </div>
      <div class="alert alert-danger alert-dismissable">
        <a href="#" class="close" data-dismiss="alert" aria-label="close">×</a>
        <strong>Danger!</strong> This alert box could indicate a dangerous or potentially negative action.
      </div>


  
Bootstrap Buttons:
------------------
To achieve the button styles above, Bootstrap has the following classes:

.btn
.btn-default
.btn-primary
.btn-success
.btn-info
.btn-warning
.btn-danger
.btn-link

  <br><br>
    <h2>Button Styles</h2>
      <button type="button" class="btn">Basic</button>
      <button type="button" class="btn btn-default">Default</button>
      <button type="button" class="btn btn-primary">Primary</button>
      <button type="button" class="btn btn-success">Success</button>
      <button type="button" class="btn btn-info">Info</button>
      <button type="button" class="btn btn-warning">Warning</button>
      <button type="button" class="btn btn-danger">Danger</button>
      <button type="button" class="btn btn-link">Link</button>   
    
    <br><br>
    <h2>Button Tags</h2>
      <a href="#" class="btn btn-info" role="button">Link Button</a>
      <button type="button" class="btn btn-info">Button</button>
      <input type="button" class="btn btn-info" value="Input Button">
      <input type="submit" class="btn btn-info" value="Submit Button">

    <br><br>
     <h2>Button Sizes</h2>
      <button type="button" class="btn btn-primary btn-lg">Large</button>
      <button type="button" class="btn btn-primary btn-md">Medium</button>    
      <button type="button" class="btn btn-primary btn-sm">Small</button>
      <button type="button" class="btn btn-primary btn-xs">XSmall</button>


    <br><br>
     <h2>Block Level Buttons</h2>
      <button type="button" class="btn btn-primary btn-block">Button 1</button>
      <button type="button" class="btn btn-default btn-block">Button 2</button>

      <h2>Large Block Level Buttons</h2>
      <button type="button" class="btn btn-primary btn-lg btn-block">Button 1</button>
      <button type="button" class="btn btn-default btn-lg btn-block">Button 2</button>

      <h2>Small Block Level Buttons</h2>
      <button type="button" class="btn btn-primary btn-sm btn-block">Button 1</button>
      <button type="button" class="btn btn-default btn-sm btn-block">Button 2</button>
    
      <br><br>
      <button type="button" class="btn btn-primary">Primary Button</button>
      <button type="button" class="btn btn-primary active">Active Primary</button>
      <button type="button" class="btn btn-primary disabled">Disabled Primary</button> 

Bootstrap Button Groups:
------------------------
Bootstrap allows you to group a series of buttons together (on a single line) in a button group:

   <br><br>
      <h2>Button Group</h2>
      <p>The .btn-group class creates a button group:</p>
      <div class="btn-group">
        <button type="button" class="btn btn-primary">Apple</button>
        <button type="button" class="btn btn-primary">Samsung</button>
        <button type="button" class="btn btn-primary">Sony</button>
      </div>

          
      <br><br> 
      <h2>Button Groups - Set Sizes</h2>
      <p>Add class .btn-group-* to size all buttons in a button group.</p>
      <h3>Large Buttons:</h3>
      <div class="btn-group btn-group-lg">
        <button type="button" class="btn btn-primary">Apple</button>
        <button type="button" class="btn btn-primary">Samsung</button>
        <button type="button" class="btn btn-primary">Sony</button>
      </div>
      <h3>Default Buttons:</h3>
      <div class="btn-group">
        <button type="button" class="btn btn-primary">Apple</button>
        <button type="button" class="btn btn-primary">Samsung</button>
        <button type="button" class="btn btn-primary">Sony</button>
      </div>
      <h3>Small Buttons:</h3>
      <div class="btn-group btn-group-sm">
        <button type="button" class="btn btn-primary">Apple</button>
        <button type="button" class="btn btn-primary">Samsung</button>
        <button type="button" class="btn btn-primary">Sony</button>
      </div>
      <h3>Extra Small Buttons:</h3>
      <div class="btn-group btn-group-xs">
        <button type="button" class="btn btn-primary">Apple</button>
        <button type="button" class="btn btn-primary">Samsung</button>
        <button type="button" class="btn btn-primary">Sony</button>
      </div> 
          
       <br><br>
       <h2>Vertical Button Group</h2>
      <p>Use the .btn-group-vertical class to create a vertical button group:</p>
      <div class="btn-group-vertical">
        <button type="button" class="btn btn-primary">Apple</button>
        <button type="button" class="btn btn-primary">Samsung</button>
        <button type="button" class="btn btn-primary">Sony</button>
      </div>   
        
      <br><br>
      <h2>Justified Button Groups</h2>
      <p>To span the entire width of the screen, use the .btn-group-justified class:</p>
      <div class="btn-group btn-group-justified">
        <a href="#" class="btn btn-primary">Apple</a>
        <a href="#" class="btn btn-primary">Samsung</a>
        <a href="#" class="btn btn-primary">Sony</a>
      </div> 
          
    <br><br>
    <h2>Justified Button Groups</h2>
      <div class="btn-group btn-group-justified">
        <div class="btn-group">
          <button type="button" class="btn btn-primary">Apple</button>
        </div>
        <div class="btn-group">
          <button type="button" class="btn btn-primary">Samsung</button>
        </div>
        <div class="btn-group">
          <button type="button" class="btn btn-primary">Sony</button>
        </div>
    </div>
    
    <br><br>
     <h2>Nesting Button Groups</h2>
      <p>Nest button groups to create drop down menus:</p>
      <div class="btn-group">
        <button type="button" class="btn btn-primary">Apple</button>
        <button type="button" class="btn btn-primary">Samsung</button>
        <div class="btn-group">
          <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
          Sony <span class="caret"></span></button>
          <ul class="dropdown-menu" role="menu">
            <li><a href="#">Tablet</a></li>
            <li><a href="#">Smartphone</a></li>
          </ul>
        </div>
      </div>
     
    <br><br>
     <h2>Split Buttons</h2>
      <div class="btn-group">
        <button type="button" class="btn btn-primary">Sony</button>
        <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
          <span class="caret"></span>
        </button>
        <ul class="dropdown-menu" role="menu">
          <li><a href="#">Tablet</a></li>
          <li><a href="#">Smartphone</a></li>
        </ul>
      </div>

Bootstrap Glyphicons:
---------------------
Glyphicons
Bootstrap provides 260 glyphicons from the Glyphicons Halflings set.
Glyphicons can be used in text, buttons, toolbars, navigation, forms, etc.
Here are some examples of glyphicons:
Envelope glyphicon: 
Print glyphicon: 
Search glyphicon: 
Download glyphicon: 


 <br><br>
     <h2>Glyphicon Examples</h2>
      <p>Envelope icon: <span class="glyphicon glyphicon-envelope"></span></p>    
      <p>Envelope icon as a link:
        <a href="#"><span class="glyphicon glyphicon-envelope"></span></a>
      </p>
      <p>Search icon: <span class="glyphicon glyphicon-search"></span></p>
      <p>Search icon on a button:
        <button type="button" class="btn btn-default">
          <span class="glyphicon glyphicon-search"></span> Search
        </button>
      </p>
      <p>Search icon on a styled button:
        <button type="button" class="btn btn-info">
          <span class="glyphicon glyphicon-search"></span> Search
        </button>
      </p>
      <p>Print icon: <span class="glyphicon glyphicon-print"></span></p>      
      <p>Print icon on a styled link button:
        <a href="#" class="btn btn-success btn-lg">
          <span class="glyphicon glyphicon-print"></span> Print 
        </a>
      </p> 

Bootstrap Badges and Labels:
----------------------------
Badges are numerical indicators of how many items are associated with a link:

News 5
Comments 10
Updates 2

The numbers (5, 10, and 2) are the badges.

Use the .badge class within <span> elements to create badges:

    <br><br>
    <h2>Badges</h2>
      <a href="#">News <span class="badge">5</span></a><br>
      <a href="#">Comments <span class="badge">10</span></a><br>
      <a href="#">Updates <span class="badge">2</span></a>
    
    <br><br>
    <h2>Badges on Buttons</h2>
      <button type="button" class="btn btn-primary">Primary <span class="badge">7</span></button>
      <button type="button" class="btn btn-success">Success <span class="badge">3</span></button>    
      <button type="button" class="btn btn-danger">Danger <span class="badge">5</span></button> 



Labels:
Labels are used to provide additional information about something:

    <br><br>
    <h2>Labels</h2>
      <h1>Example <span class="label label-default">New</span></h1>
      <h2>Example <span class="label label-default">New</span></h2>
      <h3>Example <span class="label label-default">New</span></h3>
      <h4>Example <span class="label label-default">New</span></h4>
      <h5>Example <span class="label label-default">New</span></h5>
      <h6>Example <span class="label label-default">New</span></h6>
    
    <br><br>
      <h2>Contextual Label Classes</h2>
      <p>Contextual classes can be used to color the label.</p>  
      <span class="label label-default">Default Label</span>
      <span class="label label-primary">Primary Label</span>
      <span class="label label-success">Success Label</span>
      <span class="label label-info">Info Label</span>
      <span class="label label-warning">Warning Label</span>
      <span class="label label-danger">Danger Label</span>     
          
 

Bootstrap Progress Bars:
------------------------
Basic Progress Bar
A progress bar can be used to show a user how far along he/she is in a process.

Bootstrap provides several types of progress bars.

    <br><br>
     <h2>Basic Progress Bar</h2>
      <div class="progress">
        <div class="progress-bar" role="progressbar" aria-valuenow="70" aria-valuemin="0" aria-valuemax="100" style="width:70%">
          <span class="sr-only">70% Complete</span>
        </div>
      </div>
    
    <br><br>
     <h2>Progress Bar With Label</h2>
      <div class="progress">
        <div class="progress-bar" role="progressbar" aria-valuenow="70" aria-valuemin="0" aria-valuemax="100" style="width:70%">
          70%
        </div>
      </div>
    
    <br><br>
    <h2>Colored Progress Bars</h2>
      <p>The contextual classes colors the progress bars:</p> 
      <div class="progress">
        <div class="progress-bar progress-bar-success" role="progressbar" aria-valuenow="40" aria-valuemin="0" aria-valuemax="100" style="width:40%">
          40% Complete (success)
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-info" role="progressbar" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100" style="width:50%">
          50% Complete (info)
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-warning" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width:60%">
          60% Complete (warning)
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-danger" role="progressbar" aria-valuenow="70" aria-valuemin="0" aria-valuemax="100" style="width:70%">
          70% Complete (danger)
        </div>
      </div>
    
    <br><br>
    <h2>Striped Progress Bars</h2>
      <p>The .progress-bar-striped class adds stripes to the progress bars:</p> 
      <div class="progress">
        <div class="progress-bar progress-bar-success progress-bar-striped" role="progressbar" aria-valuenow="40" aria-valuemin="0" aria-valuemax="100" style="width:40%">
          40% Complete (success)
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-info progress-bar-striped" role="progressbar" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100" style="width:50%">
          50% Complete (info)
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-warning progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width:60%">
          60% Complete (warning)
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="70" aria-valuemin="0" aria-valuemax="100" style="width:70%">
          70% Complete (danger)
        </div>
      </div>
    
     <br><br>
     <h2>Animated Progress Bar</h2>
      <p>The .active class animates the progress bar:</p> 
      <div class="progress">
        <div class="progress-bar progress-bar-striped active" role="progressbar" aria-valuenow="40" aria-valuemin="0" aria-valuemax="100" style="width:40%">
          40%
        </div>
      </div>
    
    <br><br>
    <h2>Stacked Progress Bars</h2>
      <p>Create a stacked progress bar by placing multiple bars into the same div with class .progress:</p> 
      <div class="progress">
        <div class="progress-bar progress-bar-success" role="progressbar" style="width:40%">
          Free Space
        </div>
        <div class="progress-bar progress-bar-warning" role="progressbar" style="width:10%">
          Warning
        </div>
        <div class="progress-bar progress-bar-danger" role="progressbar" style="width:20%">
          Danger
        </div>
      </div>

