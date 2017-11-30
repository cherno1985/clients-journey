# clients-journey
Find the true frequency of your retail-clients and process it from Google Analytics custom reports


#Preconditions

You have to have Google Analytics implemented in your website.
Tracking - with Enhanced E-commerce ro via events.
it really is just down to this example:

UserID | Transaction ID (Or desired Metric) | Date | Revenue

The code is built to deal with GA's report from the custom reports, in which Date column is parsed as String.
this comes into code with the function "str_to_date" (~row 16).

The problems is how to find the gaps between purchases?
especially considering that not all clients purchase the first purchase in the same day.

This code 'moves' all the purchases to 'DAY 1' of the purchase, and re-creates their purchasing Journey as per the data.

What can you do with it?
You can try and cluster same minded clinets, you can redefine and find faults in the general journey and much more, you can visualize groups of buyers (weekly, daily, monthly etc.).

