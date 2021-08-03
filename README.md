# cville_airbnb

Work on mapping all the locations of Cville AirBnB's from their website. Inclusion on the list does not mean the location is currently active, but it is still in the AirBnB registry and has not been deactivated by the owner.

# I just want the map!
Look no further than [this shiny map page](https://erinleeryan.github.io/cville_airbnbs.html). Red markers denote those AirBnBs advertising for more than 6 people. A house icon = whole home rental, a bed icon = apartment, a key icon = guesthouse and a hotel = any single address with 3 or more distinct listings.

## Homestay Regulations in the City of Charlottesville

The City of Charlottesville Homestay Regulations and Provisional Use Permit application are [here](https://www.charlottesville.gov/DocumentCenter/View/207/Homestay-Provisional-Use-Permit-PDF). These disallow non-owner-occupied short-term rentals in residential zoning, restrict owner-occupied short-term rentals to no more than 6 guests.

## Why?
Because I can. Also because it would be handy for folks in the city to have a listing and mapping of those places listed on AirBnB to compare to the licenses to see who is trying to skirt the law

## How?
Well I can't quite tell you that because a) the hope is this will be community sourced in part and b) I don't want to actually tell people listing stuff without a license how they're being stupid. Except that one dude: seriously, pay your photographer, screenshots of her proofs with all your browser tabs so you don't have to "buy" the photos is just tacky bro. I hope she learns to watermark the heck out of things.

## I want to contribute!
Awesome. The CSV file with all the data is in the data directory. The columns are:
- Address: I'm using parcel address which mostly is the same as street address except in the cases of Downtown megaparcels. Double check the name/address format with the City of [Charlottesville GIS page](https://gisweb.charlottesville.org/GisViewer/#)
- Link: the AirBnB general link for the listing. If you check your browser when looking at AirBnB for a site it'll be  _www&#46;airbnb&#46;com/rooms/\<somenumber\>_ without the spaces where <somenumber> is their unique idenfifier for the listing. We need the link through that number, but none of the other junk afterwards
  - Type: what type of rental is it? Right now I'm using __whole home__ if they're renting a house, __apartment__ if it's an apartment including a basement or attic apartment in someone's house and those apartment-like rooms in large houses that have been turned into inns such as the Belmont Farmhouse, __guesthouse__ for a detached from the main home accessory dwelling unit or guesthouse/granny flat, and __room__ if it's called out that it's just a bedroom in structure
  - guest_capacity: how many guests the listing states can use the AirBnB
  - Location_notes: if anything weird is up with the location I note it there, like places that are listed twice. Also if Hotel-like facility with room/suite numbers or names I also record that there. Also recorded here: neighborhood if I know a house and can mentally picture where it is but fail to come up with an address (if you know one of these and fill it in, thank you!)
  - Management_or_owner: there are some mega vacation management companies in town and eventually it may also be handy to see where everything is that they operate. Especially given the number of AirBnB locations owned by LLCs in this town.

  
