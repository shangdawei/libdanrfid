## Introduction ##
The code is based on the proposal for the dansk data model for RFID implementation in (public) libraries
http://www.biblev.no/RFID/dansk_rfid_datamodel.pdf

While being fairly concise about length and position of the fields, there still seems to be several ways of ordering the fields itself. This is what makes interchange of tags between different libraries impossible - sometimes even when both were equipped by the same vendor. Remember: there is a field for the library Id (aka ISIL) and even the ISO country code.

## Deeper into ISO15693 ##

http://www.ti.com/rfid/docs/manuals/refmanuals/RF-MGR-MNMN-15693-refGuide.pdf

http://focus.ti.com.cn/cn/lit/an/sloa141/sloa141.pdf

## RFID devices ##
http://cq.cx/proxmark3.pl

http://download.oracle.com/docs/cd/E13197_01/rfid/edge_server/docs20/reader_refsp1/config_use.html


## NFC ##
Although the Danish Model has nothing to do with NFC, it may well be handled by NFC devices.

http://nfc-forum.org/specs/

http://www.maintag.fr/fichiers/pdf-fr/nfcforum-ts-rtd-1-0-1.pdf

http://www.nfc-forum.org/resources/white_papers/NFC_in_Public_Transport.pdf

http://open-nfc.org/wp/editions/android/

## Focus on CRC ##