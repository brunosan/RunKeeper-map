RunKeeper-map
=============

Make a TileMill map with all the routes you have on RunKeeper


##Process

1- Download all your tracks from Runkepper
2- Export it to something [TileMill](http://mapbox.com/tilemill/) can import.
3-Import the data.
3- Customize the map look
4- Upload to Mapbox.


Insipired by [this post](http://kaseyclark.com/running-map/)


---


##1- Download all your tracks from Runkepper##

Got to the download page in your profile in [RunKeeper](http://runkeeper.com/exportData).

You´ll get a zip file on your email with the gpx tracks, and also
heartsensor data and weights IF you have used it.


##2- Export it to something [TileMill](http://mapbox.com/tilemill/) can import.i##

Convert the many gpx track to a SQLite database.

I use `ogr2ogr`. You can install it via `brew install gdl`in OSX.

ogr2ogr -f SQLite runs.sqlite RunKeeper-export/gpx/2010-11-07-1558.gpx  
