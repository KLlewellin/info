   <!DOCTYPE html>
   <html>
	<head>
		<link type="text/css" rel="stylesheet" href="../css/style.css" >
	</head>
   <body>
	   
<h1> This is a test header </h1>
	   
	   
 <!--Background image-->
 <script type="text/javascript" src="http://www.snazzyspace.com/background/background.js?script=000000_starry-skies"> </script>

var scripts = document.getElementsByTagName('script');
var myScript = scripts[ scripts.length - 1 ];

var queryString = myScript.src.replace(/^[^\?]+\??/,'');

var params = parseQuery( queryString );

function parseQuery ( query ) {
   var Params = new Object ();
   if ( ! query ) return Params; // return empty object
   var Pairs = query.split(/[;&]/);
   for ( var i = 0; i < Pairs.length; i++ ) {
      var KeyVal = Pairs[i].split('=');
      if ( ! KeyVal || KeyVal.length != 2 ) continue;
      var key = unescape( KeyVal[0] );
      var val = unescape( KeyVal[1] );
      val = val.replace(/\+/g, ' ');
      Params[key] = val;
   }
   return Params;
}
   
   
 <!--Right below is an image of the sun-->
 <img id="sun" src="http://www.heywhatsthat.com/images/planets/1000/sun.png">

		
 <!--Insert the 'earth' on the next line-->
 <!--Make the earth a child of its own orbit-->
 
 <div id="earth-orbit">
            <img id="earth" src="http://2.bp.blogspot.com/_ZnSBvB1XKlM/SMQz2GlvscI/AAAAAAAAAIo/zghbJ6z8eWg/s320/cat_icon_internet_256.png">
        </div>
 

 <!--Other stuff: Change the sun and earth images, Add all the planets! Animate the sun's glow-->
 <div id = "mars-orbit">
            <img id = "mars" src="http://www.heywhatsthat.com/images/planets/1000/mars.png">
        </div>
<div id = "venus-orbit">
            <img id = "venus" src="http://endeavour.pegasusfleet.net/images/ClassN22.png">
        </div>
<div id = "mercury-orbit">
            <img id = "mercury" src="http://star.arm.ac.uk/eu-unawe/docs/Print%20Package/05%20Planet%20Images/images/Mod_4_Image_2_mercury_NASA.png">
        </div>
      

   </body>
 </html>
	
    
