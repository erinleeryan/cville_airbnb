# cville_airbnb
Work on mapping all the locations of Cville Air BnB's from their website

## Why?
Because I can. Also because it would be handy for folks in the city to have a listing and mapping of those places listed on AirBnB to compare to the licenses to see who is trying to skirt the law

## How?
Well I can't quite tell you that because a) the hope is this will be community sourced in part and b) I don't want to actually tell people listing stuff without a license how they're being stupid. Except that one dude: seriously, pay your photographer, screenshots of her proofs with all your browser tabs so you don't have to "buy" the photos is just tacky bro. I hope she learns to watermark the heck out of things.

## I want to contribute!
Awesome. The CSV file with all the data is in the data directory. The columns are:
- Address: I'm using parcel address which mostly is the same as street address except in the cases of Downtown megaparcels. Double check the name/address format with the City of [Charlottesville GIS page] (https://gisweb.charlottesville.org/GisViewer/#)
- Link: the AirBnB general link for the listing. If you check your browser when looking at AirBnB for a site it'll be _www.airbnb.com/rooms/<somenumber>_ where <somenumber> is their unique idenfifier for the listing. We need the link through that number, but none of the other junk afterwares
  - Type: what type of rental is it? Right now I'm using __whole house__ if they're renting a house, __apartment__ if it's an apartment, __basement apt__ if it's a basement apartment in someone's house, __upstairs apt__ for the folks who are renting a self contained upstairs of their house, __accessory dwelling__ for an accessory dwelling or guesthouse or __Suite__ if it's like a hotel room where there's multiple rooms at a single address and there's nothing like a kitchen to cook in
  - Location-y notes: if anything weird is up with the location I note it there, like places that are listed twice. Also if Hotel-like facility with room/suite numbers or names I also record that there. Also recorded here: neighborhood if I know a house and can mentally picture where it is but fail to come up with an address (if you know one of these and fill it in, thank you!)
  - Management/Owner: there are some mega vacation management companies in town and eventually it may also be handy to see where everything is that they operate. Especially given the number of AirBnB locations owned by LLCs in this town.
