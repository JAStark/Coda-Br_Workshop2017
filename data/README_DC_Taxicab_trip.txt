TITLE: Taxicab Trip Information

ABSTRACT:  DC Taxi trips from May 2015 to March 2017.  The zip file contains zip files of pipe (|) delimeted text files for trips by month.  The record counts are:

Month		Count
5/2015		1,397,102 
6/2015		1,470,466 
7/2015		1,401,792 
8/2015		1,129,707 
9/2015		1,308,445 
10/2015		1,487,133 
11/2015	 	  993,502 
12/2015		1,081,726 
1/2016	 	  922,338 
2/2016		1,194,698 
3/2016		1,404,639 
4/2016		1,369,882 
5/2016		1,323,155 
6/2016		1,282,651 
7/2016		1,109,118 
8/2016		  949,650 
9/2016		1,203,388 
10/2016		1,027,036 
11/2016		1,011,673 
12/2016	 	  898,993 
1/2017	  	  901,807 
2/2017	 	  949,578 
3/2017		1,237,621 


DISCLAIMER: The data provided herein is derived from electronic sources the accuracy of which cannot be guaranteed. While DFHV strives to provide data that is accurate and current, all data provided is for informational purposes only. The District of Columbia disclaims all liability for errors, omissions, completeness, accuracy and currentness of the data provided herein. Use of data provided herein constitutes acceptance of these terms.

CATEGORY: Public Service	

PROVIDER: Office of the Chief Technology Officer (OCTO)

ORIGINATOR: Department of For-Hire Vehicles (DFHV)

PROCESS DESCRIPTION: DFHV provided OCTO with a taxicab trip text file representing trips from May 2015 to March 2017.  OCTO processed the data to assign a block locations to pick up and drop off locations.  The blocks were assigned using the original pick up, drop off lat/long coordinates and searching for the block locations in the DC Master Address Repository (radius tolerance of 250 meters and less).  The pick and drop off times were also rounded to the nearest hour.
In addition, the pick up and drop off locations were assigned to an airport using locator polygons for Reagan, BWI, and Dulles.  These polygons generally followed the visual borders of these airports.
The block assignment metrics are as follows
 
				Pick Up Location	Drop Off Location	   
Total Records:	           	 27,196,432	            27,196,432    
Percent Geocoded to block:	    83%	              		78%	    
			 
For more information, go to http://dfhv.dc.gov

TABLE STRUCTURE:

COLUMN_NAME		DATA_TYPE	DEFINITION	   
OBJECTID		NUMBER(9)	Table Unique Identifier	   
TRIPTYPE		VARCHAR2(255)	Type of Taxi Trip	   
PROVIDER		VARCHAR2(255)	Taxi Company that Provided trip	   
METERFARE		VARCHAR2(255)	Meter Fare	   
TIP			VARCHAR2(255)	Tip amount	   
SURCHARGE		VARCHAR2(255)	Surcharge fee	   
EXTRAS			VARCHAR2(255)	Extra fees	   
TOLLS			VARCHAR2(255)	Toll amount	   
TOTALAMOUNT		VARCHAR2(255)	Total amount from Meter fare, tip, surcharge, extras, and tolls. 	   
PAYMENTTYPE		VARCHAR2(255)	Payment type	   
PAYMENTCARDPROVIDER	VARCHAR2(255)	Payment card provider	   
PICKUPCITY		VARCHAR2(255)	Pick up location city	   
PICKUPSTATE		VARCHAR2(255)	Pick up location state	   
PICKUPZIP		VARCHAR2(255)	Pick up location zip	   
DROPOFFCITY		VARCHAR2(255)	Drop off location city	   
DROPOFFSTATE		VARCHAR2(255)	Drop off location state	   
DROPOFFZIP		VARCHAR2(255)	Drop off location zip	   
TRIPMILEAGE		VARCHAR2(255)	Trip milaege	   
TRIPTIME		VARCHAR2(255)	Trip time	   
PICKUP_BLOCK_LATITUDE	NUMBER		Pick up location latitude	   
PICKUP_BLOCK_LONGITUDE	NUMBER		Pick up location longitude	   
PICKUP_BLOCKNAME	VARCHAR2(255)	Pick up location street block name	   
DROPOFF_BLOCK_LATITUDE	NUMBER		Drop off location latitude	   
DROPOFF_BLOCK_LONGITUDE	NUMBER		Drop off location longitude	   
DROPOFF_BLOCKNAME	VARCHAR2(255)	Drop off location street block name	   
AIRPORT			CHAR(1)		Pick up or drop off location is a local airport (Y/N)	   
PICKUPDATETIME_TR	DATE		Pick up location city	   
DROPOFFDATETIME_TR	DATE		Drop off location city	 

