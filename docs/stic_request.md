# stic_request

## Request

#### sender ([Identifiers Australian Business Number Identifier](https://definitions.ausdx.io/definition/trc/de26)): string

A unique public identifier issued to all entities registered in the Australian Business Register (ABR), to be used in their dealings with government. Companies registered under the Corporations Law and business entities carrying on an enterprise in Australia are entitled to an ABN.



#### requestor ([Identifiers Australian Business Number Identifier](https://definitions.ausdx.io/definition/trc/de26)): string

A unique public identifier issued to all entities registered in the Australian Business Register (ABR), to be used in their dealings with government. Companies registered under the Corporations Law and business entities carrying on an enterprise in Australia are entitled to an ABN.



#### abn ([Identifiers Australian Business Number Identifier](https://definitions.ausdx.io/definition/trc/de26)): string

A unique public identifier issued to all entities registered in the Australian Business Register (ABR), to be used in their dealings with government. Companies registered under the Corporations Law and business entities carrying on an enterprise in Australia are entitled to an ABN.



#### action ([Interaction Reason Text](https://definitions.ausdx.io/definition/trc/de13082)): string

Information describing the reason for an interaction as required by the receiving agency.



#### responseCode ([ResponseCode](https://ausdx-lab.herokuapp.com/define/de007)): int

Another code to indicate the success or failure of the request

The HTTP response code for this request.
For more information, see [wikipedia](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)



Check the wikipedia article for specific meanings of each code, but in general:

- 1xx are Informational responses
-	2xx are Success
-	3xx are Redirection
-	4xx are Client errors
-	5xx are Server errors



#### person: [Person](#person)

#### address: [Address](#address)

#### account: [Account](#account)

#### geo: [Geo](#geo)


## Geo

#### somethingNew ([Address Details Geocode Latitude Number](https://definitions.ausdx.io/definition/fs/de13091)): float

The geographic latitude of a point on the earth is a measurement in degrees north or south of the equator reference to a prescribed datum.  Latitudes south of the equator are expressed as a negative number, north of the equator as positive.



Usage Example: -33.91277417




## Account

#### accountNumber ([Identifiers Superannuation Member Account Identifier](https://definitions.ausdx.io/definition/trc/de7461)): string

This is a unique number used to identify a superannuation member account.



#### accountStatus ([Superannuation Fund Details Member Account Status Code](https://definitions.ausdx.io/definition/trc/de7393)): string

This indicates the status of the member's superannuation account.



Valid values are:
Lost = The member is lost due to not being contactable with an account balance that is greater than zero.
Inactive = The member is lost due to inactivity with an account balance greater than zero.
Found = The member was previously reported as lost or inactive and has re-established contact. 
Transferred = The member was previously reported as lost or inactive and has transferred to another super provider or the Tax Office as unclaimed monies. 
Error = The member was previously reported in error.
Open =  The member's account is open and the fund will accept payments.
Closed = The member's account is closed and will not accept payments.
Where a member is both inactive and lost, the member should be reported as 'Lost'.



#### accountStatusDate ([Superannuation Fund Details Member Account Status Date](https://definitions.ausdx.io/definition/trc/de13995)): string

The date the member's superannuation account status was updated.



#### usi ([Superannuation Fund Details Unique Superannuation Identifier](https://definitions.ausdx.io/definition/trc/de7395)): string

The unique superannuation identifier is used for identifying the product within the fund which the member account belongs to.




## Person

#### tfn ([Identifiers Tax File Number Identifier](https://definitions.ausdx.io/definition/trc/de27)): string

A unique number issued by the Tax Office to individuals and organisations to identify their tax records. It increases the efficiency in administering tax and other Australian Government systems such as income support payments. It is also used as the identifier for clients' income tax roles. A Tax File Number (TFN) can be used externally only for communication with the Tax Office, either directly by the client, or by an external organisation that is required to collect and quote the client's TFN to the Tax Office.



#### dayOfBirth ([Person Demographic Details Birth DayofMonth](https://definitions.ausdx.io/definition/trc/de13055)): string

The date of the day in the month in which an individual was born



#### monthOfBirth ([Person Demographic Details Birth Month](https://definitions.ausdx.io/definition/trc/de13056)): string

The month in which an individual was born



#### yearOfBirth ([Person Demographic Details Birth Year](https://definitions.ausdx.io/definition/trc/de13057)): string

The year in which an individual was born



#### surname ([Person Name Details Family Name Text](https://definitions.ausdx.io/definition/trc/de40)): string

The person's last name or surname. The name by which a family group is identified.



#### givenName ([Person Name Details Given Name Text](https://definitions.ausdx.io/definition/trc/de41)): string

The name given to a person which is that person's identifying name within the family group or the name by which the person is uniquely socially identified; the name borne by an individual, often assigned by his or her parents shortly after birth, as opposed to the inherited surname.



#### middleName ([Person Name Details Other Given Name Text](https://definitions.ausdx.io/definition/trc/de42)): string

The middle name given to a person which complements that person's identifying name within the family group or the name by which the person is uniquely socially identified.




## Address

#### line1 ([Address Details Line 1 Text](https://definitions.ausdx.io/definition/trc/de17)): string

First line utilising free format, that is used to create a semi structured address.



#### line2 ([Address Details Line 2 Text](https://definitions.ausdx.io/definition/trc/de18)): string

Second line utilising free format, that is used to create a semi structured address.



#### suburb ([Address Details Locality Name Text](https://definitions.ausdx.io/definition/trc/de19)): string

A word or combination of words, by which a geographic locality/suburb is designated or known.



#### postcode ([Address Details Postcode Text](https://definitions.ausdx.io/definition/trc/de21)): string

The Australian descriptor for a postal delivery area, aligned with locality, suburb or place



#### state ([Address Details State Or Territory Code](https://definitions.ausdx.io/definition/trc/de22)): string

The code that is assigned to each Australian State or Territory



#### country ([Address Details Country Code](https://definitions.ausdx.io/definition/trc/de15)): string

This represents the Country Code as prescribed by AS4590 and inherited from ISO 3166




