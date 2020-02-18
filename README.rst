polanie.prv.pl-mirror
=====================

See https://github.com/jstasiak/polanie-resources for other Polanie resources.

What is this?
-------------

http://polanie.prv.pl/ is a site by Janusz "Swoosh" Prokulewicz. The site
is about `Polanie <https://en.wikipedia.org/wiki/Polanie_(video_game)>`_ – 
a Polish real-time strategy game released in 1996.

The site contains some valuable resources (save games, editors, patches,
tutorials, unit and structure information, game and editor source code etc.)
and it seems that it's the only place where one can find them. This mirror
is an effort to preserve the site's contents in case the original site goes
down.

How was it created?
-------------------

::

   httrack polanie.prv.pl

Then prv.pl-injected ads, tracking code and other annoyances have been
removed::

   cd polanie.prv.pl
   rm prv_hosting_footer.js prv_site_config_values.js
   find . -type f -name '*.html' | xargs sed -i 's/<!-- End \/\/]]>.*//g'

+ some manual edits

The mirror has been created at 2019-02-01.

How can I use this mirror?
--------------------------

1. Download the repository (using Git or in a ZIP)
2. Open ``polanie.prv.pl/index.html``
