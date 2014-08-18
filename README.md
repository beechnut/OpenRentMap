Open Rent Map
=============

"A tool for seeing each other, our neighbors, in our experience of gentrification." - @allthesignals

Inspired by the [continuing][continuing] [gentrification][gentrification] [and][and] [displacement][displacement] [in][in] [Boston][Boston].


[continuing]: http://www.bostonglobe.com/metro/regionals/north/2014/07/16/letter-keeping-somerville-union-square-affordable-must-combined-effort/KjA9GTQVhB0S8CDrW7OmMO/story.html
[gentrification]: http://www.theguardian.com/cities/2014/jul/10/helsinki-shared-public-transport-plan-car-ownership-pointless?CMP=twt_gu
[and]: http://marshfield.wickedlocal.com/article/20140718/NEWS/140716251/?Start=1
[displacement]: http://www.bostonglobe.com/lifestyle/2014/08/16/skyrocketing-rent-has-tenants-searching-outside-city/UHNF9rzXPaperduj5dchFI/story.html
[in]: http://www.bostonglobe.com/business/2014/07/21/mass-condo-market-hotter-than-ever/wQShpMpF46I0PPQZWgDL9I/story.html
[Boston]: http://www.sparechangenews.net/news/priced-development-drives-rising-rents-union-square/

This map will be a tool for understand rents across the city, and how much landlords and realtors profit off of rents.


### Roadmap

+ Create a GeoJSON tile layer from the statewide parcel database. The tile layer should include attributes ID and Address.

+ Create a JSON API (using Rails) that will fetch attribute data from  

+ Build a front-end application that implements the following workflow:

    1. Scroll across the map or enter your address.
    2. Click on your parcel.
    3. A window pops up with the address. Confirm that this is your address, or cancel and find the correct parcel.
    4. Confirm the number of units, or edit the number.
    5. Check whether someone else has entered your unit. If so, you can still contribute your information.
    6. Enter your unit's floor area. (Direct them to where this might be found on a lease.)
    7. Enter the rent for your unit, or for the whole building if you know it.
    8. Enter the monthly cost of utilities your landlord pays for (usually water, sometimes electricity).
    9. Enter the cost of repairs, renovations, or other services your landlord provides.
    10. (Optionally) Enter your email if you want to learn of any findings that come out of the data.
    11. View a summary of data, including an estimate (with methodology) of how much your landlord earns in rent, and how much profit they make after property taxes, utilities, and repairs.


### Design Ideas

+ Might use splash images from [unsplash.it](http://unsplash.it), probably just city-themed ones:

![Random image from unsplash.it](http://unsplash.it/730/185?random)

+ Parcels will be each assigned one of a set [very][very] [vibrant][vibrant] colors. When a parcel has no user-contributed data, it is completely grayscale (unsaturated). It gets more saturated as a function of the proportion of units for which users contribute data. Data-rich areas will be [brilliant](http://wmgardner.co/agemap/index.html), whereas data-poor areas will be [bland](http://tiles.mapc.org/#17/42.35527/-71.06016).

[very]: https://kuler.adobe.com/very-vibrant-color-theme-1163277/
[vibrant]: https://kuler.adobe.com/vibrant-color-theme-274696/


