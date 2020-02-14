 Creating Interactive Images in MadCap Flare

I'll be honest, I've only recently discovered HTML image maps and it just so happens that there is a handy tool in Flare for creating them.
To me, image maps hark back to a long forgotten time of whacky, off-the-wall web design and you don't see many examples of them these days. I worry that there is a reason for this and I've yet to discover it.
Anyway, here's how I made some nice interactive images in Flare using HTML image maps and some JQuery plugins.
In my projects, I create a master page to handle scripts. In this example, I keep it simple and show all code being added to a single topic. 

There are a few JQuery plugins at work here:
 - ImageMapster
 - Hilight
 - Tooltip

To use these in your project, insert the following into the `<head>` of your  image map topic:

      <link href="https://code.jquery.com/ui/1.10.4/themes/ui-lightness/jquery-ui.css" rel="stylesheet" />
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js">
        </script>
        <script src="http://www.outsharked.com/scripts/jquery.imagemapster.js">
        </script>
        <script src="https://code.jquery.com/ui/1.10.4/jquery-ui.js">
        </script>
Now you might run into some trouble as Flare might insert the JQuery library during your build. If you find your image map isn't working, try removing this from your build or making sure this one loads first, and then your image mapping plugins load after.

    <script src="../Resources/Scripts/jquery.min.js" type="text/javascript">
    </script> 

