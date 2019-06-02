# hardcodeMVC
Custom MVC




## Firstly
1. Rename the htaccess files, which is in hardcodemvc folder, in public folder and finally in app folder, to .htaccess, for server configuration.
2. Rename "hardcodemvc" in RewriteBase /hardcodemvc/public in the htaccess file which is in public folder, to your project name (e.g /yourprojectname/public)



## Usage
By default, /pages/index is default route, which is defined in libraries/Core.php. 
'pages' is controller, which is a class in app/Controllers/ and 'index' is method in the controller.

When user requests www.hardcodemvc.com/, if he does not have session, this default route runs and load the view 'index.php' in app/views/pages/.
If he has session, he is redirected to your home page.

1. To load view, inside the corresponding controller, call 
``` $this->view('pages/index', $data)```. 
$data is optional. If you have some data to tell the user in the view, you can pass it in the view method.
```$this->view('pages/index', $data)``` loads the index.php which is in /app/views/pages/.

2. Mostly, you will work with 
  * /app/controllers/
  * /app/models/
  * /app/views/


## Demo
To better see how it works, check out [this repo](https://github.com/HtetPhyoHPN/sharepost).
