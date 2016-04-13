-----------------------------------------------------
How Can XML be Used?

Date: 2016-04-13

-----------------------------------------------------

XML is used in many aspects of Web development; often used to separate data from presentation.

1, XML Separates Data from Presentation

  * XML does not carry any information about how to be displayed.
  * the same XML data can be used in many different presentation scenarios.
  * with XML, there is a full separation between **data** and **presentation**.

2, XML is often a Complement of HTML

  * In many HTML applications, XML is used to **store or transport** data, while HTML is used to **format and display** the
  same data.

3, XML separates data from HTML

  * When display data in HTML, you should not have to edit the HTML file when the data changes.
  * With XML, the data can be stored in separate XML files.
  * With a few lines of JavaScript code, you can read an XML file and upate the data content of any HTML page.

4, Next, will learn a lot more about using XML and JavaScript in the DOM section.

```
<?xml version="1.0" encoding="UTF-8"?>
<bookstore>

  <book category="cooking">
    <title lang="en">Everyday Italian</title>
    <author>Giada De Laurentiis</author>
    <year>2005</year>
    <price>30.00</price>
  </book>

  <book category="children">
    <title lang="en">Harry Potter</title>
    <author>J K. Rowling</author>
    <year>2005</year>
    <price>29.99</price>
  </book>

  <book category="web">
    <title lang="en">XQuery Kick Start</title>
    <author>James McGovern</author>
    <author>Per Bothner</author>
    <author>Kurt Cagle</author>
    <author>James Linn</author>
    <author>Vaidyanathan Nagarajan</author>
    <year>2003</year>
    <price>49.99</price>
  </book>

  <book category="web" cover="paperback">
    <title lang="en">Learning XML</title>
    <author>Erik T. Ray</author>
    <year>2003</year>
    <price>39.95</price>
  </book>

</bookstore>
```

5, Transaction Data

  * Thousands of XML formats exists, in many different industries, to describe day\-to\-day transactions.
    * Stocks and shares
    * Financial Transactions
    * Medical Data
    * Mathematical data
    * Scientific Measurements
    * News Information
    * Weather Services
  
  * Example 1
  
  ```
  <?xml version="1.0" encoding="UTF-8"?>
  <nitf>
    <head>
      <title>Colombia Earthquake</title>
    </head>
    <body>
      <headline>
        <hl1>143 Dead in Colombia Earthquake</hl1>
      </headline>
      <byline>
        <bytag>By Jared Kotler, Associated Press Writer</bytag>
      </byline>
      <dateline>
        <location>Bogota, Colombia</location>
        <date>Monday January 25 1999 7:28 ET</date>
      </dateline>
    </body>
  </nitf>
  ```
  
  * Example 2
  
  ```
  <?xml version="1.0" encoding="UTF-8"?>
  <current_observation>
  
  <credit>NOAA's National Weather Service</credit>
  <credit_URL>http://weather.gov/</credit_URL>
  
  <image>
    <url>http://weather.gov/images/xml_logo.gif</url>
    <title>NOAA's National Weather Service</title>
    <link>http://weather.gov</link>
  </image>
  
  <location>New York/John F. Kennedy Intl Airport, NY</location>
  <station_id>KJFK</station_id>
  <latitude>40.66</latitude>
  <longitude>-73.78</longitude>
  <observation_time_rfc822>Mon, 11 Feb 2008 06:51:00 -0500 EST
  </observation_time_rfc822>
  
  <weather>A Few Clouds</weather>
  <temp_f>11</temp_f>
  <temp_c>-12</temp_c>
  <relative_humidity>36</relative_humidity>
  <wind_dir>West</wind_dir>
  <wind_degrees>280</wind_degrees>
  <wind_mph>18.4</wind_mph>
  <wind_gust_mph>29</wind_gust_mph>
  <pressure_mb>1023.6</pressure_mb>
  <pressure_in>30.23</pressure_in>
  <dewpoint_f>-11</dewpoint_f>
  <dewpoint_c>-24</dewpoint_c>
  <windchill_f>-7</windchill_f>
  <windchill_c>-22</windchill_c>
  <visibility_mi>10.00</visibility_mi>
  
  <icon_url_base>http://weather.gov/weather/images/fcicons/</icon_url_base>
  <icon_url_name>nfew.jpg</icon_url_name>
  <disclaimer_url>http://weather.gov/disclaimer.html</disclaimer_url>
  <copyright_url>http://weather.gov/disclaimer.html</copyright_url>
  
  </current_observation>
  ```
