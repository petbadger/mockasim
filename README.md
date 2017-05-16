# mockasim
##### For creating mock data for simulations and testing.

### Randomly Generated Canadian Postal Codes
---

One of the more significant functions of mockasim is a function that generates random Canadian Postal Codes.

#### About Canadian Postal Codes (CPC)
---

_Note that postal codes do change every year. A couple hundred could be added, depracated or revived and possibly not even represent the same geographic location._

Canadian postal codes are comprised of six characters and allow for mail to be mechanically, and manually, sorted for easier mail delivery to specific geographic locations. Currently there are approximately 850,000 postal codes in Canada with an average of 14 households in each.
All Canadian postal codes follow the same format and are divided into two three-character segments:

A#A #A#
(letter-number-letter-space-number-letter-number)

However, in the wild, Postal Codes will often not have a space, replace the space with a hyphen, contain lowercase and more (for example, on questionnaires or customer databases).

The first segment is called the 'forward sortation area' (FSA) and is used to identify the geographic location of the address. The first character of the FSA represents the 'postal district', which splits the country into major geographic regions.
The first letter of the FSA uniquely identifies the province or territory, except in a few cases to be explained later. Each province or territory has one or more identifying letters, as follows:

    A 	    Newfoundland and Labrador
    B 		Nova Scotia
    C 		Prince Edward Island
    E 		New Brunswick
    G 		Québec East
    H 		Montréal Metropolitan
    J 		Québec West
    K 		Eastern Ontario
    L 		Central Ontario
    M 		Toronto
    N 		Southwestern Ontario
    P 		Northern Ontario
    R 		Manitoba
    S 		Saskatchewan
    T 		Alberta
    V 		British Columbia
    X 		Northwest Territories and Nunavut
    Y 		Yukon Territory 

The letters can be thought of as advancing from east (A) to west (V) across the provinces, then east (X) to west (Y) again across the territories to the north. The east-to-west association is not geographically perfect, especially in the Maritime Provinces to the east, but it is close enough to be mnemonically useful. 

The second character is used to separate rural and urban regions. The number '0' denotes a rural region with numbers 1 through 9 representing urban areas. It's common for rural regions to be 'urbanized', which involves the changing of the '0' to another number. The third character is used to more precisely describe the geographic area of the address.

The second segment is called the 'location delivery unit' (LDU) and represents either a specific address or group of addresses. Sometimes an LDU covers an entire city block, all (or part) of a high-rise, a small rural community or even a single house.

The following letters never appear in a Canadian postal code:
    D    F    I    O    Q    U 
    W and Z also do not appear as the first letter of a CPC

There are only two CPCs that start with H0 (other than the fictitious H0H 0H0 for Santa Clause at the North Pole) and none that start with M0. This makes sense if you think about the role of 0 identifying a rural area, and the role of H and M identifying the very non-rural Montréal and Toronto areas.

More information can be found on the Canada Post website: https://www.canadapost.ca/tools/pg/manual/PGaddress-e.asp
Special thanks to http://www.columbia.edu/~fdc/postal/postal-ca.html


#### Future Functions
The ability to create a dataset with a range of random socio-demographic data such as Age, Gender, Location, and Likert Scales.

