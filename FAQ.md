## Whats the goal? ##

Ths library shall provide a reference implementation dealing with the different implementations of the [Danish Data Model](http://www.biblev.no/RFID/dansk_rfid_datamodel.pdf). While providing a quite strict definition, tags often cannot be interchanged between institutions. If there were a reference implementation, vendors could easily check compliance of their model against it.

## What is Danish on the Danish Model? ##

Denmarks Library widely use RFID ("near NfcV" ;-) tags providing a high level of automation for checkout and return operations. Happily most of them use a common standard - later on called the danish one. Read more about this standard [here](http://www.bibliotheksportal.de/themen/rfid/normung.html). ISO 28560-3 describing the facts being, was published in March 2011. At that time NFC was established already.
A more detailed view written by the authors of the danish model, already addressing interlibrary loan is  [here](http://biblstandard.dk/rfid/docs/summary.htm) at http://biblstandard.dk/rfid/. The differences between the current implementation and ISO 28560-3 are addressed at http://biblstandard.dk/rfid/dk/iso28560versusdsinf163.pdf

# Where's the code? #

Well - there are two classes visible up to now. One dealing with the payload itself and another implementing the CRC, which is essential for discriminating between valid tags and other payload.

Another class DDMFindings inspects the payload in order to find design issues on tags "in the wild". Different vendors produce - slightly - different tags, while all pretend to implement the Danish Data Model. The differences will prevent a seamless cross-reading experience which will be necessary, if RFID shall ever play a role in InterLibrary Loan.

Meanwhile there is an Android App **RFID Validator** analyzing given tags.


A small commandline tool for block layout generation will follow soon.