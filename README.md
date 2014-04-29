sac data co-op
==============
This repo is like a 'mission control' for some local data gathering and mapping projects I'm working on. Collaborators are welcome! 

Hoping to map all sorts of things here. So far, we're starting with food pantries!

## Food Pantries

#### Goal: Add Sacramento-area food pantries and food kitchens to Open Street Map. 

**Why:** Open Street Map is free, open source, and lots of neat tools are available to help people make their own maps with it.

**Target Outcomes:** Hopefully, other people will make use of this data by sharing it/mapping it/incorporating it into apps, so that people who need food can get it and not go hungry. Would also be great to help people learn about how to make use of Open Street Map data because it's free for everyone and its maps are beautiful.

### How to help:
#### Collect lists of places that need to be mapped.
Add them to the to-do list [here](https://github.com/haileypate/sac-data/issues?labels=things-to-map&state=open). <br>

#### Add places from the list to Open Street Map.
One way is to use the [Id editor](http://www.openstreetmap.org/). <br>

If the places already exist (food pantries are often held in community buildings used for other things), tag them with "community\_resource: food_pantry" and maybe add a note about where to find more info.<br>

### Getting the data:

One way to get data out of Open Street Map is to head over to the [Overpass API](http://overpass-turbo.eu/). To grab the list of food pantries we've found in the Sacramento region, enter the following query:
```
<query type="node">
  <has-kv k="community_resource" v="food_pantry"/>
  <bbox-query w="-121.82100" s="38.39500" e="-120.99500" n="38.95500"/>
</query>
<print/>
```

### Mapping the food pantries:

There are a number of ways to make maps with OSM data. One option is to use take advantage of the map hosting on this GitHub account, which can be found [here](https://gist.github.com/haileypate/aca4f44b3b8aa6e041b2). You can embed a the most current version of the map into your website by adding the following line of code: 
```
<script src="https://gist.github.com/haileypate/aca4f44b3b8aa6e041b2.js"></script>
```


