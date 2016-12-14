# Fake News Detector (or a data source to build one)

A node script uses which data from [this](https://docs.google.com/spreadsheets/d/1xDDmbr54qzzG8wUrRdxQl_C1dixJSIYqQUaXVZBqsJs) Google sheet, preprocesses it for cleanup and dumps it to a JSON file. What use will this be, you might ask? Well, I think this is a good starting point for developers to build apps/tools that could benefit from a fake news detection facility, or for data analysis purposes.

The possibilities are endless. I am putting this on Github in a hope that we might be able to improve upon this with more nice things, such as feeding this data this data into Firebase endpoint and enable REST API access. Please modify this code however you wish. Damage might have been done, but we can do something.

### Dependencies 

`"csvtojson": "^1.0.3"`

### Installation 

`npm install`

### Running

` sudo node src/convert-csv-to-json.js`

### Things To Do

* Feed data into Firebase 
* Create REST API endpoint
    * That allows user to query by specific URL 
    * That allows user to query by rank in a defined order
    * That allows user(s) to add more sites to the existing collection 
        * Which means, a UI for public moderation to prevent trolling becomes necessary

For submitting your ideas, contact me on [Facebook](https://www.facebook.com/ali.gajani)

### Output

```
[{
	"siteTitle": "100PercentFedUp",
	"siteCategory": "clickbait",
	"siteUrl": "100PercentFedUp.com",
	"siteGoogleHits": 137000,
	"siteFacebookLikes": 1005880,
	"siteTwitterFollowers": 11600,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "21st Century Wire",
	"siteCategory": "conspiracy",
	"siteUrl": "http://21stcenturywire.com/",
	"siteGoogleHits": 161000,
	"siteFacebookLikes": 21096,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": "Syria backed?"
}, {
	"siteTitle": "369News",
	"siteCategory": "conspiracy",
	"siteUrl": "369news.net/",
	"siteGoogleHits": 37400,
	"siteFacebookLikes": 5866,
	"siteTwitterFollowers": 1441,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "70news",
	"siteCategory": "clickbait",
	"siteUrl": "https://70news.wordpress.com/",
	"siteGoogleHits": 257000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "A Sheep No More",
	"siteCategory": "conspiracy",
	"siteUrl": "http://asheepnomore.net/",
	"siteGoogleHits": 219000,
	"siteFacebookLikes": 256066,
	"siteTwitterFollowers": 901,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "Abcnews.com.co",
	"siteCategory": "fake news",
	"siteUrl": "http://abcnews.com.co/",
	"siteGoogleHits": 11100000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Accuracy in Media (AIM)",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.aim.org/",
	"siteGoogleHits": 244000,
	"siteFacebookLikes": 11836,
	"siteTwitterFollowers": 22400,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "ACN Latitudes",
	"siteCategory": "junk science",
	"siteUrl": "http://latitudes.org/",
	"siteGoogleHits": 27600,
	"siteFacebookLikes": 1611,
	"siteTwitterFollowers": 26500,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "ActivistPost",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.activistpost.com/",
	"siteGoogleHits": 571000,
	"siteFacebookLikes": 542095,
	"siteTwitterFollowers": 23700,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Addicting Info",
	"siteCategory": "clickbait",
	"siteUrl": "http://addictinginfo.org/",
	"siteGoogleHits": 616000,
	"siteFacebookLikes": 1231596,
	"siteTwitterFollowers": 21300,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "AdwNews",
	"siteCategory": "conspiracy",
	"siteUrl": "http://awdnews.com/",
	"siteGoogleHits": 13400,
	"siteFacebookLikes": 1762,
	"siteTwitterFollowers": 4375,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "Age of Autism",
	"siteCategory": "junk science",
	"siteUrl": "http://www.ageofautism.com/",
	"siteGoogleHits": 344000,
	"siteFacebookLikes": 16663,
	"siteTwitterFollowers": 33000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Allen B. West",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.allenbwest.com/",
	"siteGoogleHits": 232000,
	"siteFacebookLikes": 1324011,
	"siteTwitterFollowers": 586000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Allen West Republic",
	"siteCategory": "clickbait",
	"siteUrl": "http://allenwestrepublic.com/",
	"siteGoogleHits": 249000,
	"siteFacebookLikes": 752172,
	"siteTwitterFollowers": 23400,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Alt Health Works",
	"siteCategory": "junk science",
	"siteUrl": "http://althealthworks.com/",
	"siteGoogleHits": 91900,
	"siteFacebookLikes": 154882,
	"siteTwitterFollowers": 1253,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Alternet",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.alternet.org/",
	"siteGoogleHits": 2560000,
	"siteFacebookLikes": 926893,
	"siteTwitterFollowers": 122000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Amandla! Media",
	"siteCategory": "clickbait",
	"siteUrl": "http://aidc.org.za/",
	"siteGoogleHits": 2210000,
	"siteFacebookLikes": 5443,
	"siteTwitterFollowers": 1668,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "AmericaBlog",
	"siteCategory": "clickbait",
	"siteUrl": "http://americablog.com/",
	"siteGoogleHits": 623000,
	"siteFacebookLikes": 10205,
	"siteTwitterFollowers": 15600,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "American Enterprise Institute",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.aei.org/",
	"siteGoogleHits": 605000,
	"siteFacebookLikes": 272972,
	"siteTwitterFollowers": 67200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "American Free Press",
	"siteCategory": "conspiracy",
	"siteUrl": "http://americanfreepress.net/",
	"siteGoogleHits": 225000,
	"siteFacebookLikes": 2161,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "American Freedom Fighters",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.americasfreedomfighters.com/",
	"siteGoogleHits": 73600,
	"siteFacebookLikes": 445053,
	"siteTwitterFollowers": 5296,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "American Lookout",
	"siteCategory": "clickbait",
	"siteUrl": "http://americanlookout.com/",
	"siteGoogleHits": 21500000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 1409,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "American News",
	"siteCategory": "conspiracy",
	"siteUrl": "http://americannews.com/",
	"siteGoogleHits": 4530000,
	"siteFacebookLikes": 5483682,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "American News X",
	"siteCategory": "clickbait",
	"siteUrl": "http://americannewsx.com/",
	"siteGoogleHits": 40100,
	"siteFacebookLikes": 234298,
	"siteTwitterFollowers": 1368,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "American Renaissance",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.amren.com/",
	"siteGoogleHits": 3330000,
	"siteFacebookLikes": 5471,
	"siteTwitterFollowers": 15000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "American Spectator",
	"siteCategory": "clickbait",
	"siteUrl": "https://spectator.org/",
	"siteGoogleHits": 651000,
	"siteFacebookLikes": 109303,
	"siteTwitterFollowers": 33700,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "American Thinker",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.americanthinker.com/",
	"siteGoogleHits": 844000,
	"siteFacebookLikes": 111814,
	"siteTwitterFollowers": 35300,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "American Updater",
	"siteCategory": "clickbait",
	"siteUrl": "http://americanupdater.com/",
	"siteGoogleHits": 397000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Americans for Prosperity",
	"siteCategory": "clickbait",
	"siteUrl": "https://americansforprosperity.org/",
	"siteGoogleHits": 417000,
	"siteFacebookLikes": 1116622,
	"siteTwitterFollowers": 130000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "AmplifyingGlass",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.amplifyingglass.com/",
	"siteGoogleHits": 26200,
	"siteFacebookLikes": 23142,
	"siteTwitterFollowers": 1562,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "AnonNews",
	"siteCategory": "",
	"siteUrl": "http://www.anonews.co/",
	"siteGoogleHits": 123000,
	"siteFacebookLikes": 35668,
	"siteTwitterFollowers": 103000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Another Day in the Empire",
	"siteCategory": "conspiracy",
	"siteUrl": "http://anotherdayintheempire.com/",
	"siteGoogleHits": 8070,
	"siteFacebookLikes": 315,
	"siteTwitterFollowers": 9670,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Answers in Genesis",
	"siteCategory": "hate",
	"siteUrl": "https://answersingenesis.org/",
	"siteGoogleHits": 492000,
	"siteFacebookLikes": 436923,
	"siteTwitterFollowers": 46500,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Anti-War",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.antiwar.com/",
	"siteGoogleHits": 26100000,
	"siteFacebookLikes": 64690,
	"siteTwitterFollowers": 33000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Awareness Act",
	"siteCategory": "conspiracy",
	"siteUrl": "http://awarenessact.com/",
	"siteGoogleHits": 395000,
	"siteFacebookLikes": 958410,
	"siteTwitterFollowers": 176,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Baltimore Gazette",
	"siteCategory": "",
	"siteUrl": "http://baltimoregazette.com/",
	"siteGoogleHits": 475000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Baptist News Global",
	"siteCategory": "clickbait",
	"siteUrl": "https://baptistnews.com/",
	"siteGoogleHits": 24300,
	"siteFacebookLikes": 6389,
	"siteTwitterFollowers": 5836,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Bare Naked Islam",
	"siteCategory": "",
	"siteUrl": "http://www.barenakedislam.com/",
	"siteGoogleHits": 330000,
	"siteFacebookLikes": 2608,
	"siteTwitterFollowers": 16900,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Bay Area Reporter",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.ebar.com/",
	"siteGoogleHits": 127000,
	"siteFacebookLikes": 11104,
	"siteTwitterFollowers": 3105,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "BB4SP",
	"siteCategory": "clickbait",
	"siteUrl": "http://bb4sp.com/",
	"siteGoogleHits": 159000,
	"siteFacebookLikes": 182644,
	"siteTwitterFollowers": 103000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Before It’s News",
	"siteCategory": "conspiracy",
	"siteUrl": "http://beforeitsnews.com/",
	"siteGoogleHits": 2570000,
	"siteFacebookLikes": 393557,
	"siteTwitterFollowers": 62900,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Big Blue Vision",
	"siteCategory": "clickbait",
	"siteUrl": "http://bigbluevision.com/",
	"siteGoogleHits": 7120,
	"siteFacebookLikes": 15084,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Big Government News",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.biggovernment.news/",
	"siteGoogleHits": 28900000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "BigPZone aka therundownlive aka wearechange",
	"siteCategory": "clickbait",
	"siteUrl": "http://therundownlive.com/",
	"siteGoogleHits": 15200,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 859,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Bipartisan Report",
	"siteCategory": "clickbait",
	"siteUrl": "http://bipartisanreport.com/",
	"siteGoogleHits": 502000,
	"siteFacebookLikes": 1092373,
	"siteTwitterFollowers": 209000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "BizPac Review",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.bizpacreview.com/",
	"siteGoogleHits": 277000,
	"siteFacebookLikes": 2483275,
	"siteTwitterFollowers": 40800,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Black Genocide",
	"siteCategory": "conspiracy",
	"siteUrl": "blackgenocide.org",
	"siteGoogleHits": 140000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Blue Lives Matter",
	"siteCategory": "clickbait",
	"siteUrl": "http://bluelivesmatter.blue/",
	"siteGoogleHits": 694000,
	"siteFacebookLikes": 1312085,
	"siteTwitterFollowers": 199000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Blue Nation Review",
	"siteCategory": "clickbait",
	"siteUrl": "http://bluenationreview.com/",
	"siteGoogleHits": 74100,
	"siteFacebookLikes": 1037304,
	"siteTwitterFollowers": 58,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Borowitz Report",
	"siteCategory": "satire",
	"siteUrl": "http://www.newyorker.com/humor/borowitz-report",
	"siteGoogleHits": 163000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 586542,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Breitbart",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.breitbart.com/",
	"siteGoogleHits": 9880000,
	"siteFacebookLikes": 2855869,
	"siteTwitterFollowers": 502000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Bust Magazine",
	"siteCategory": "clickbait",
	"siteUrl": "http://bust.com/",
	"siteGoogleHits": 247000,
	"siteFacebookLikes": 133256,
	"siteTwitterFollowers": 62000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Call the Cops",
	"siteCategory": "satire",
	"siteUrl": "http://www.callthecops.net/",
	"siteGoogleHits": 371000,
	"siteFacebookLikes": 17242,
	"siteTwitterFollowers": 485,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Canada Free Press",
	"siteCategory": "clickbait",
	"siteUrl": "http://canadafreepress.com/",
	"siteGoogleHits": 289000,
	"siteFacebookLikes": 16225,
	"siteTwitterFollowers": 11310,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Canadian Dimension",
	"siteCategory": "clickbait",
	"siteUrl": "https://canadiandimension.com/",
	"siteGoogleHits": 51300,
	"siteFacebookLikes": 4009,
	"siteTwitterFollowers": 2386,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Cap News",
	"siteCategory": "satire",
	"siteUrl": "http://cap-news.com/",
	"siteGoogleHits": 162000,
	"siteFacebookLikes": 1654,
	"siteTwitterFollowers": 4084,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Center For American Progress",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.americanprogress.org/",
	"siteGoogleHits": 523000,
	"siteFacebookLikes": 78559,
	"siteTwitterFollowers": 62100,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Center for Media and Democracy",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.prwatch.org/",
	"siteGoogleHits": 828000,
	"siteFacebookLikes": 58696,
	"siteTwitterFollowers": 9445,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Center for Security Policy",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.centerforsecuritypolicy.org/",
	"siteGoogleHits": 356000,
	"siteFacebookLikes": 21742,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Charisma News",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.charismanews.com/",
	"siteGoogleHits": 372000,
	"siteFacebookLikes": 181644,
	"siteTwitterFollowers": 14800,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Chicago Reader",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.chicagoreader.com/",
	"siteGoogleHits": 763000,
	"siteFacebookLikes": 77148,
	"siteTwitterFollowers": 204000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Chicks on the Right",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.chicksontheright.com/",
	"siteGoogleHits": 1670000,
	"siteFacebookLikes": 1075712,
	"siteTwitterFollowers": 37300,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Christian Post",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.christianpost.com/",
	"siteGoogleHits": 1450000,
	"siteFacebookLikes": 181644,
	"siteTwitterFollowers": 151664,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Christian Times Newspaper",
	"siteCategory": "clickbait",
	"siteUrl": "http://christiantimesnewspaper.com/",
	"siteGoogleHits": 60400,
	"siteFacebookLikes": 525,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "christwire",
	"siteCategory": "satire",
	"siteUrl": "http://christwire.org/",
	"siteGoogleHits": 50600,
	"siteFacebookLikes": 16731,
	"siteTwitterFollowers": 1081,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Chronicle.su",
	"siteCategory": "satire",
	"siteUrl": "http://chronicle.su/",
	"siteGoogleHits": 550000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 28000,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "Chronicles (Rockford Institute)",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.chroniclesmagazine.org/",
	"siteGoogleHits": 119000,
	"siteFacebookLikes": 1979,
	"siteTwitterFollowers": 1527,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Citizens United",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.citizensunited.org/",
	"siteGoogleHits": 1910000,
	"siteFacebookLikes": 437566,
	"siteTwitterFollowers": 17800,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "City Journal",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.city-journal.org/",
	"siteGoogleHits": 1780000,
	"siteFacebookLikes": 52850,
	"siteTwitterFollowers": 21100,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Clash Daily",
	"siteCategory": "clickbait",
	"siteUrl": "http://clashdaily.com/",
	"siteGoogleHits": 473000,
	"siteFacebookLikes": 52850,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "ClickHole",
	"siteCategory": "satire",
	"siteUrl": "http://www.clickhole.com/",
	"siteGoogleHits": 588000,
	"siteFacebookLikes": 600819,
	"siteTwitterFollowers": 262000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "CNS News",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.cnsnews.com/",
	"siteGoogleHits": 1110000,
	"siteFacebookLikes": 2067996,
	"siteTwitterFollowers": 110000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Coast to Coast AM",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.coasttocoastam.com/",
	"siteGoogleHits": 601000,
	"siteFacebookLikes": 412976,
	"siteTwitterFollowers": 120000,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "CollectiveEvolution",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.collective-evolution.com/",
	"siteGoogleHits": 2550000,
	"siteFacebookLikes": 4855177,
	"siteTwitterFollowers": 61600,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Collectively Conscious",
	"siteCategory": "conspiracy",
	"siteUrl": "http://collectivelyconscious.net/",
	"siteGoogleHits": 199000,
	"siteFacebookLikes": 383304,
	"siteTwitterFollowers": 817,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Commentary Magazine",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.commentarymagazine.com/",
	"siteGoogleHits": 260000,
	"siteFacebookLikes": 49952,
	"siteTwitterFollowers": 22400,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Common Dreams",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.commondreams.org/",
	"siteGoogleHits": 1270000,
	"siteFacebookLikes": 48800,
	"siteTwitterFollowers": 360923,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Conscious Life News",
	"siteCategory": "junk science",
	"siteUrl": "http://consciouslifenews.com/",
	"siteGoogleHits": 332000,
	"siteFacebookLikes": 1100898,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Conservapedia",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.conservapedia.com/",
	"siteGoogleHits": 278000,
	"siteFacebookLikes": 10400,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Conservative 101",
	"siteCategory": "clickbait",
	"siteUrl": "https://conservative101.com/",
	"siteGoogleHits": 452000,
	"siteFacebookLikes": 1685838,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Conservative Daily Post",
	"siteCategory": "conspiracy",
	"siteUrl": "https://conservativedailypost.com/",
	"siteGoogleHits": 3650000,
	"siteFacebookLikes": 448838,
	"siteTwitterFollowers": 316,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Conservative HQ",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.conservativehq.com/",
	"siteGoogleHits": 38500,
	"siteFacebookLikes": 1431,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Conservative Outfitters",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.conservativeoutfitters.com/",
	"siteGoogleHits": 58300,
	"siteFacebookLikes": 17655,
	"siteTwitterFollowers": 11800,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Conservative Post",
	"siteCategory": "clickbait",
	"siteUrl": "http://conservativepost.com/",
	"siteGoogleHits": 442000,
	"siteFacebookLikes": 1430815,
	"siteTwitterFollowers": 504,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Conservative Review",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.conservativereview.com/",
	"siteGoogleHits": 672000,
	"siteFacebookLikes": 1484445,
	"siteTwitterFollowers": 67100,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Conservative Spirit",
	"siteCategory": "clickbait",
	"siteUrl": "http://conservativespirit.com/",
	"siteGoogleHits": 6180,
	"siteFacebookLikes": 5659,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Conservative Tribune",
	"siteCategory": "clickbait",
	"siteUrl": "http://conservativetribune.com/",
	"siteGoogleHits": 1240000,
	"siteFacebookLikes": 3319110,
	"siteTwitterFollowers": 75000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Conspiracy Planet",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.conspiracyplanet.com/",
	"siteGoogleHits": 29900,
	"siteFacebookLikes": 361,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Constitution Rising",
	"siteCategory": "clickbait",
	"siteUrl": "http://rickwells.us/",
	"siteGoogleHits": 20900,
	"siteFacebookLikes": 60915,
	"siteTwitterFollowers": 28000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Controversial Times",
	"siteCategory": "clickbait",
	"siteUrl": "http://controversialtimes.com/",
	"siteGoogleHits": 38500,
	"siteFacebookLikes": 5316,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "CountdownToZeroTime",
	"siteCategory": "conspiracy",
	"siteUrl": "http://countdowntozerotime.com/",
	"siteGoogleHits": 11000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Counter Current News",
	"siteCategory": "conspiracy",
	"siteUrl": "http://countercurrentnews.com/",
	"siteGoogleHits": 257000,
	"siteFacebookLikes": 403378,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "CounterPsyOps",
	"siteCategory": "conspiracy",
	"siteUrl": "https://counterpsyops.com/",
	"siteGoogleHits": 13700,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 1563,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "CounterPunch",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.counterpunch.org/",
	"siteGoogleHits": 1760000,
	"siteFacebookLikes": 91629,
	"siteTwitterFollowers": 43100,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "CreamBMP",
	"siteCategory": "satire",
	"siteUrl": "http://creambmp.com/",
	"siteGoogleHits": 39100,
	"siteFacebookLikes": 64779,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Crime Prevention Research Center",
	"siteCategory": "clickbait",
	"siteUrl": "http://crimeresearch.org/",
	"siteGoogleHits": 1070000,
	"siteFacebookLikes": 4780,
	"siteTwitterFollowers": 925,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Crooks and Liars",
	"siteCategory": "clickbait",
	"siteUrl": "http://crooksandliars.com/",
	"siteGoogleHits": 558000,
	"siteFacebookLikes": 115879,
	"siteTwitterFollowers": 56100,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "CS Globe",
	"siteCategory": "conspiracy",
	"siteUrl": "http://csglobe.com/",
	"siteGoogleHits": 40100,
	"siteFacebookLikes": 13956,
	"siteTwitterFollowers": 558,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Daily Caller",
	"siteCategory": "clickbait",
	"siteUrl": "http://dailycaller.com/",
	"siteGoogleHits": 3210000,
	"siteFacebookLikes": 3769844,
	"siteTwitterFollowers": 239000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Daily Dot",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.dailydot.com/",
	"siteGoogleHits": 2240000,
	"siteFacebookLikes": 2345551,
	"siteTwitterFollowers": 276000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Daily Headlines",
	"siteCategory": "conspiracy",
	"siteUrl": "http://dailyheadlines.net/",
	"siteGoogleHits": 1950000,
	"siteFacebookLikes": 309452,
	"siteTwitterFollowers": 63,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Daily Kos",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.dailykos.com/",
	"siteGoogleHits": 3580000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 8444,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Daily News Bin",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.dailynewsbin.com/",
	"siteGoogleHits": 46900,
	"siteFacebookLikes": 63764,
	"siteTwitterFollowers": 28300,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Daily Signal",
	"siteCategory": "clickbait",
	"siteUrl": "http://dailysignal.com/",
	"siteGoogleHits": 702000,
	"siteFacebookLikes": 656924,
	"siteTwitterFollowers": 38700,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Daily Wire",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.dailywire.com/",
	"siteGoogleHits": 742000,
	"siteFacebookLikes": 1388088,
	"siteTwitterFollowers": 21600,
	"sitePoliticalAlignment": "centre",
	"siteNotes": ""
}, {
	"siteTitle": "DailyBuzzLive",
	"siteCategory": "satire",
	"siteUrl": "http://dailybuzzlive.com/",
	"siteGoogleHits": 71400,
	"siteFacebookLikes": 195476,
	"siteTwitterFollowers": 108000,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "DailyCurrant",
	"siteCategory": "satire",
	"siteUrl": "http://dailycurrant.com/",
	"siteGoogleHits": 93200,
	"siteFacebookLikes": 86044,
	"siteTwitterFollowers": 5531,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "DailyOccupation",
	"siteCategory": "",
	"siteUrl": "http://dailyoccupation.com/",
	"siteGoogleHits": 74000000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "DailySnark",
	"siteCategory": "satire",
	"siteUrl": "http://dailysnark.com/",
	"siteGoogleHits": 92000,
	"siteFacebookLikes": 24500,
	"siteTwitterFollowers": 178,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Dallas Voice",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.dallasvoice.com/",
	"siteGoogleHits": 159000,
	"siteFacebookLikes": 10333,
	"siteTwitterFollowers": 19100,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Data Asylum",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.dataasylum.com/",
	"siteGoogleHits": 11400,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 171,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "David Horowitz Freedom Center",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.horowitzfreedomcenter.org/",
	"siteGoogleHits": 46100,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 1901,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "David Wolfe",
	"siteCategory": "junk science",
	"siteUrl": "https://www.davidwolfe.com/",
	"siteGoogleHits": 4110000,
	"siteFacebookLikes": 8548023,
	"siteTwitterFollowers": 88000,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "DC Gazette",
	"siteCategory": "conspiracy",
	"siteUrl": "http://thedcgazette.com/",
	"siteGoogleHits": 144000,
	"siteFacebookLikes": 423332,
	"siteTwitterFollowers": 3103,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "DCClothesLine",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.dcclothesline.com/",
	"siteGoogleHits": 207000,
	"siteFacebookLikes": 108309,
	"siteTwitterFollowers": 13900,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Democratic Underground",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.democraticunderground.com/",
	"siteGoogleHits": 976000,
	"siteFacebookLikes": 75033,
	"siteTwitterFollowers": 7469,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Denver Guardian",
	"siteCategory": "",
	"siteUrl": "-",
	"siteGoogleHits": 546000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "DerfMagazine",
	"siteCategory": "satire",
	"siteUrl": "http://www.derfmagazine.com/",
	"siteGoogleHits": 5710,
	"siteFacebookLikes": 4048,
	"siteTwitterFollowers": 7628,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "Disclose TV",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.disclose.tv/",
	"siteGoogleHits": 819000,
	"siteFacebookLikes": 1993665,
	"siteTwitterFollowers": 37500,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Discover the Networks",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.discoverthenetworks.org/",
	"siteGoogleHits": 384000,
	"siteFacebookLikes": 3115,
	"siteTwitterFollowers": 652,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Discovery Institute",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.discovery.org/",
	"siteGoogleHits": 400000,
	"siteFacebookLikes": 7006,
	"siteTwitterFollowers": 659,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Dissent Magazine",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.dissentmagazine.org/",
	"siteGoogleHits": 118000,
	"siteFacebookLikes": 23453,
	"siteTwitterFollowers": 34400,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Downtrend",
	"siteCategory": "clickbait",
	"siteUrl": "http://downtrend.com/",
	"siteGoogleHits": 1950000,
	"siteFacebookLikes": 151206,
	"siteTwitterFollowers": 1921,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Drudge Report",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.drudgereport.com/",
	"siteGoogleHits": 1840000,
	"siteFacebookLikes": 1130862,
	"siteTwitterFollowers": 1100000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "DuffleBlog",
	"siteCategory": "satire",
	"siteUrl": "http://www.duffelblog.com/",
	"siteGoogleHits": 111000,
	"siteFacebookLikes": 255672,
	"siteTwitterFollowers": 20346,
	"sitePoliticalAlignment": "centrist",
	"siteNotes": ""
}, {
	"siteTitle": "Eagle Rising",
	"siteCategory": "clickbait",
	"siteUrl": "http://eaglerising.com/",
	"siteGoogleHits": 306000,
	"siteFacebookLikes": 658259,
	"siteTwitterFollowers": 4415,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Economy in Crisis",
	"siteCategory": "clickbait",
	"siteUrl": "http://economyincrisis.org/",
	"siteGoogleHits": 334000,
	"siteFacebookLikes": 95,
	"siteTwitterFollowers": 2784,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "EcoWatch",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.ecowatch.com/",
	"siteGoogleHits": 579000,
	"siteFacebookLikes": 191992,
	"siteTwitterFollowers": 126000,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Educate-Yourself",
	"siteCategory": "conspiracy",
	"siteUrl": "http://educate-yourself.org/",
	"siteGoogleHits": 5080000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Electronic Intifada",
	"siteCategory": "clickbait",
	"siteUrl": "https://electronicintifada.net/",
	"siteGoogleHits": 438000,
	"siteFacebookLikes": 80700,
	"siteTwitterFollowers": 169994,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Embols",
	"siteCategory": "clickbait",
	"siteUrl": "http://embols.com/",
	"siteGoogleHits": 262000,
	"siteFacebookLikes": 7476,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Empire Herald",
	"siteCategory": "fake news",
	"siteUrl": "https://empireherald.com/",
	"siteGoogleHits": 21700,
	"siteFacebookLikes": 43711,
	"siteTwitterFollowers": 165000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Empire News",
	"siteCategory": "satire",
	"siteUrl": "http://empirenews.net/",
	"siteGoogleHits": 462000,
	"siteFacebookLikes": 21884,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "EmpireSports.co",
	"siteCategory": "satire",
	"siteUrl": "http://www.empiresports.co/",
	"siteGoogleHits": 152000,
	"siteFacebookLikes": 3202,
	"siteTwitterFollowers": 477,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Ending the Fed News",
	"siteCategory": "conspiracy",
	"siteUrl": "http://endingthefed.com/",
	"siteGoogleHits": 77400,
	"siteFacebookLikes": 358922,
	"siteTwitterFollowers": 187,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "EnduringVision",
	"siteCategory": "satire",
	"siteUrl": "http://www.enduringvision.com/",
	"siteGoogleHits": 341000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 78,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "Everyday Feminism",
	"siteCategory": "clickbait",
	"siteUrl": "http://everydayfeminism.com/",
	"siteGoogleHits": 419000,
	"siteFacebookLikes": 521499,
	"siteTwitterFollowers": 69400,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Family Research Council",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.frc.org/",
	"siteGoogleHits": 434000,
	"siteFacebookLikes": 192666,
	"siteTwitterFollowers": 24400,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Family Security Matters",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.familysecuritymatters.org/",
	"siteGoogleHits": 156000,
	"siteFacebookLikes": 8262,
	"siteTwitterFollowers": 694,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Federalist Press",
	"siteCategory": "clickbait",
	"siteUrl": "http://federalistpress.com/mission",
	"siteGoogleHits": 7530,
	"siteFacebookLikes": 3426,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Food Babe",
	"siteCategory": "junk science",
	"siteUrl": "http://foodbabe.com/",
	"siteGoogleHits": 545000,
	"siteFacebookLikes": 1143658,
	"siteTwitterFollowers": 102000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Forward Progressives",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.forwardprogressives.com/",
	"siteGoogleHits": 157000,
	"siteFacebookLikes": 349211,
	"siteTwitterFollowers": 6107,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Fox News",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.foxnews.com/",
	"siteGoogleHits": 19400000,
	"siteFacebookLikes": 13999658,
	"siteTwitterFollowers": 11900000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Freakout Nation",
	"siteCategory": "clickbait",
	"siteUrl": "http://freakoutnation.com/",
	"siteGoogleHits": 179000,
	"siteFacebookLikes": 322157,
	"siteTwitterFollowers": 8844,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Freedom Daily",
	"siteCategory": "clickbait",
	"siteUrl": "http://freedomdaily.com/",
	"siteGoogleHits": 532000,
	"siteFacebookLikes": 1519778,
	"siteTwitterFollowers": 11900,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Freedom Outpost",
	"siteCategory": "clickbait",
	"siteUrl": "http://freedomoutpost.com/",
	"siteGoogleHits": 290000,
	"siteFacebookLikes": 2009,
	"siteTwitterFollowers": 105362,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Freedom Works",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.freedomworks.org/",
	"siteGoogleHits": 153000,
	"siteFacebookLikes": 4844252,
	"siteTwitterFollowers": 261000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Freethought Project",
	"siteCategory": "clickbait",
	"siteUrl": "http://thefreethoughtproject.com/",
	"siteGoogleHits": 533000,
	"siteFacebookLikes": 1733579,
	"siteTwitterFollowers": 10000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "From the Trenches World Report",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.fromthetrenchesworldreport.com/",
	"siteGoogleHits": 48000,
	"siteFacebookLikes": 249,
	"siteTwitterFollowers": 204,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Frontpage Magazine",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.frontpagemag.com/",
	"siteGoogleHits": 430000,
	"siteFacebookLikes": 36560,
	"siteTwitterFollowers": 6538,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Future in America",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.futureinamerica.com/",
	"siteGoogleHits": 188000,
	"siteFacebookLikes": 694661,
	"siteTwitterFollowers": 2096,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "GeoEngineering Watch",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.geoengineeringwatch.org/",
	"siteGoogleHits": 285000,
	"siteFacebookLikes": 27013,
	"siteTwitterFollowers": 2805,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Global Research",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.globalresearch.ca/",
	"siteGoogleHits": 5690000,
	"siteFacebookLikes": 241233,
	"siteTwitterFollowers": 21900,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "GomerBlog",
	"siteCategory": "satire",
	"siteUrl": "http://gomerblog.com/",
	"siteGoogleHits": 98600,
	"siteFacebookLikes": 159190,
	"siteTwitterFollowers": 11208,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Gone Left",
	"siteCategory": "clickbait",
	"siteUrl": "http://goneleft.com/",
	"siteGoogleHits": 131000,
	"siteFacebookLikes": 94206,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Government Accountability Institute",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.g-a-i.org/",
	"siteGoogleHits": 7290,
	"siteFacebookLikes": 12743,
	"siteTwitterFollowers": 9549,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Government Slaves",
	"siteCategory": "conspiracy",
	"siteUrl": "http://govtslaves.info/",
	"siteGoogleHits": 22000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 2031,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Greenville Gazette",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.greenvillegazette.com/",
	"siteGoogleHits": 212000,
	"siteFacebookLikes": 833321,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Groopspeak",
	"siteCategory": "clickbait",
	"siteUrl": "http://news.groopspeak.com/",
	"siteGoogleHits": 199000,
	"siteFacebookLikes": 493524,
	"siteTwitterFollowers": 641,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Guardian Liberty Voice",
	"siteCategory": "clickbait",
	"siteUrl": "http://guardianlv.com/",
	"siteGoogleHits": 270000,
	"siteFacebookLikes": 3557,
	"siteTwitterFollowers": 2326,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Gulag Bound",
	"siteCategory": "conspiracy",
	"siteUrl": "http://gulagbound.com/",
	"siteGoogleHits": 32100,
	"siteFacebookLikes": 3083,
	"siteTwitterFollowers": 20400,
	"sitePoliticalAlignment": "Right",
	"siteNotes": ""
}, {
	"siteTitle": "Hang the Bankers",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.hangthebankers.com/",
	"siteGoogleHits": 106000,
	"siteFacebookLikes": 17613,
	"siteTwitterFollowers": 10200,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Health Eternally",
	"siteCategory": "junk science",
	"siteUrl": "http://healtheternally.com/",
	"siteGoogleHits": 530000,
	"siteFacebookLikes": 10048,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Health Impact News",
	"siteCategory": "junk science",
	"siteUrl": "https://healthimpactnews.com/",
	"siteGoogleHits": 249000,
	"siteFacebookLikes": 477349,
	"siteTwitterFollowers": 59300,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Health Nut News",
	"siteCategory": "junk science",
	"siteUrl": "http://www.healthnutnews.com/",
	"siteGoogleHits": 204000,
	"siteFacebookLikes": 432629,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Health Sciences Institute",
	"siteCategory": "junk science",
	"siteUrl": "http://hsionline.com/",
	"siteGoogleHits": 381000,
	"siteFacebookLikes": 10123,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Heartland Institute",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.heartland.org/",
	"siteGoogleHits": 296000,
	"siteFacebookLikes": 100569,
	"siteTwitterFollowers": 12800,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Heritage Foundation",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.heritage.org/",
	"siteGoogleHits": 4820000,
	"siteFacebookLikes": 530,
	"siteTwitterFollowers": 57200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Hot Air",
	"siteCategory": "clickbait",
	"siteUrl": "http://hotair.com/",
	"siteGoogleHits": 45100000,
	"siteFacebookLikes": 828052,
	"siteTwitterFollowers": 13100,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Hudson Institute",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.hudson.org/",
	"siteGoogleHits": 582000,
	"siteFacebookLikes": 9009,
	"siteTwitterFollowers": 28400,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Human Events",
	"siteCategory": "clickbait",
	"siteUrl": "http://humanevents.com/",
	"siteGoogleHits": 1190000,
	"siteFacebookLikes": 744961,
	"siteTwitterFollowers": 31600,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Humans Are Free",
	"siteCategory": "conspiracy",
	"siteUrl": "http://humansarefree.com/",
	"siteGoogleHits": 386000,
	"siteFacebookLikes": 35396,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Huzlers",
	"siteCategory": "satire",
	"siteUrl": "http://huzlers.com/",
	"siteGoogleHits": 56400,
	"siteFacebookLikes": 7183,
	"siteTwitterFollowers": 6897,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "I have the Truth",
	"siteCategory": "clickbait",
	"siteUrl": "https://ihavethetruth.com/",
	"siteGoogleHits": 79300,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "I Love My Freedom",
	"siteCategory": "clickbait",
	"siteUrl": "http://ilovemyfreedom.org/",
	"siteGoogleHits": 337000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "If You Only News",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.ifyouonlynews.com/",
	"siteGoogleHits": 81000,
	"siteFacebookLikes": 569002,
	"siteTwitterFollowers": 781,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "IJR(Independent Journal Review)",
	"siteCategory": "",
	"siteUrl": "http://ijr.com/",
	"siteGoogleHits": 328000,
	"siteFacebookLikes": 441182,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "centre-right",
	"siteNotes": ""
}, {
	"siteTitle": "Illuminati News",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.illuminati-news.com/",
	"siteGoogleHits": 96100,
	"siteFacebookLikes": 3391,
	"siteTwitterFollowers": 4567,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "In These Times",
	"siteCategory": "clickbait",
	"siteUrl": "http://inthesetimes.com/",
	"siteGoogleHits": 11300000,
	"siteFacebookLikes": 75831,
	"siteTwitterFollowers": 20700,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Infinite Unknown",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.infiniteunknown.net/",
	"siteGoogleHits": 81800,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 176,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Infowars",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.infowars.com/",
	"siteGoogleHits": 4910000,
	"siteFacebookLikes": 630491,
	"siteTwitterFollowers": 191000,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Inquisitr",
	"siteCategory": "",
	"siteUrl": "http://www.inquisitr.com/",
	"siteGoogleHits": 7520000,
	"siteFacebookLikes": 3006077,
	"siteTwitterFollowers": 54400,
	"sitePoliticalAlignment": "centrist/left",
	"siteNotes": "Multinews aggregator"
}, {
	"siteTitle": "Institute for Creation Research (IRC)",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.icr.org/",
	"siteGoogleHits": 1470000,
	"siteFacebookLikes": 136403,
	"siteTwitterFollowers": 5428,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Institute for Responsible Technology",
	"siteCategory": "conspiracy",
	"siteUrl": "http://responsibletechnology.org/",
	"siteGoogleHits": 378000,
	"siteFacebookLikes": 111756,
	"siteTwitterFollowers": 6354,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Intellihub",
	"siteCategory": "conspiracy",
	"siteUrl": "https://www.intellihub.com/",
	"siteGoogleHits": 128000,
	"siteFacebookLikes": 28269,
	"siteTwitterFollowers": 21200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "iTagLive",
	"siteCategory": "",
	"siteUrl": "https://itaglive.com/",
	"siteGoogleHits": 435,
	"siteFacebookLikes": 42,
	"siteTwitterFollowers": 3,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Jacobin",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.jacobinmag.com/",
	"siteGoogleHits": 2090000,
	"siteFacebookLikes": 210496,
	"siteTwitterFollowers": 91400,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Jihad Watch",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.jihadwatch.org/",
	"siteGoogleHits": 597000,
	"siteFacebookLikes": 50829,
	"siteTwitterFollowers": 54400,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "JonesReport",
	"siteCategory": "conspiracy",
	"siteUrl": "http://jonesreport.com/",
	"siteGoogleHits": 90500,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Jookos News",
	"siteCategory": "clickbait",
	"siteUrl": "http://jookosnews.tumblr.com/",
	"siteGoogleHits": 1180,
	"siteFacebookLikes": 65648,
	"siteTwitterFollowers": 1022,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Judicial Watch",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.judicialwatch.org/",
	"siteGoogleHits": 1690000,
	"siteFacebookLikes": 3410932,
	"siteTwitterFollowers": 365000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Knowledge of Today",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.knowledgeoftoday.org/",
	"siteGoogleHits": 85700,
	"siteFacebookLikes": 1160982,
	"siteTwitterFollowers": 11400,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Knox Report",
	"siteCategory": "clickbait",
	"siteUrl": "http://knoxreport.com/",
	"siteGoogleHits": 26800000,
	"siteFacebookLikes": 7879,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Lavender Magazine",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.lavendermagazine.com/",
	"siteGoogleHits": 35000,
	"siteFacebookLikes": 11486,
	"siteTwitterFollowers": 6524,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Left Action",
	"siteCategory": "clickbait",
	"siteUrl": "http://leftaction.com/",
	"siteGoogleHits": 441000,
	"siteFacebookLikes": 1287723,
	"siteTwitterFollowers": 28700,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Lew Rockwell",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.lewrockwell.com/",
	"siteGoogleHits": 532000,
	"siteFacebookLikes": 103552,
	"siteTwitterFollowers": 48200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Liberal America",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.liberalamerica.org/",
	"siteGoogleHits": 456000,
	"siteFacebookLikes": 694190,
	"siteTwitterFollowers": 8526,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Liberals Unite (Samuel Warde)",
	"siteCategory": "clickbait",
	"siteUrl": "http://samuel-warde.com/",
	"siteGoogleHits": 482000,
	"siteFacebookLikes": 200343,
	"siteTwitterFollowers": 1710,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Liberty Alliance",
	"siteCategory": "clickbait",
	"siteUrl": "http://libertyalliance.com/",
	"siteGoogleHits": 356000,
	"siteFacebookLikes": 72141,
	"siteTwitterFollowers": 3596,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Liberty News",
	"siteCategory": "conspiracy",
	"siteUrl": "http://libertynews.com/",
	"siteGoogleHits": 279000,
	"siteFacebookLikes": 1429985,
	"siteTwitterFollowers": 7205,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Liberty Unyielding",
	"siteCategory": "clickbait",
	"siteUrl": "http://libertyunyielding.com/",
	"siteGoogleHits": 129000,
	"siteFacebookLikes": 92500,
	"siteTwitterFollowers": 1882,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Liberty Videos",
	"siteCategory": "conspiracy",
	"siteUrl": "http://libertyvideos.org/",
	"siteGoogleHits": 20600,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 1226,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Liberty Writers News",
	"siteCategory": "clickbait",
	"siteUrl": "http://libertywritersnews.com/",
	"siteGoogleHits": 42200,
	"siteFacebookLikes": 832462,
	"siteTwitterFollowers": 41300,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "LibertyTalk.FM",
	"siteCategory": "clickbait",
	"siteUrl": "http://libertytalk.fm/",
	"siteGoogleHits": 36800,
	"siteFacebookLikes": 10152,
	"siteTwitterFollowers": 195,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "LifeZette",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.lifezette.com/",
	"siteGoogleHits": 729000,
	"siteFacebookLikes": 668892,
	"siteTwitterFollowers": 20200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Live Free Live Natural",
	"siteCategory": "junk science",
	"siteUrl": "https://www.facebook.com/livefreelivenatural/",
	"siteGoogleHits": 31500,
	"siteFacebookLikes": 37325,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "LMR/LibertyMovementRadio",
	"siteCategory": "",
	"siteUrl": "http://libertymovementradio.com/",
	"siteGoogleHits": 5370,
	"siteFacebookLikes": 2457,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Manchester Union Leader",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.unionleader.com/",
	"siteGoogleHits": 46600,
	"siteFacebookLikes": 14341,
	"siteTwitterFollowers": 39700,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Media Matters",
	"siteCategory": "clickbait",
	"siteUrl": "https://mediamatters.org/",
	"siteGoogleHits": 1420000,
	"siteFacebookLikes": 665434,
	"siteTwitterFollowers": 245000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Media Research Center",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.mrc.org/",
	"siteGoogleHits": 458000,
	"siteFacebookLikes": 1562273,
	"siteTwitterFollowers": 150000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Media Zone",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.mediazone.com.hk/",
	"siteGoogleHits": 1070000,
	"siteFacebookLikes": 3046,
	"siteTwitterFollowers": 7865,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Mediaite",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.mediaite.com/",
	"siteGoogleHits": 1550000,
	"siteFacebookLikes": 225217,
	"siteTwitterFollowers": 123000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "MediaMass",
	"siteCategory": "celebrity",
	"siteUrl": "http://en.mediamass.net/",
	"siteGoogleHits": 685000,
	"siteFacebookLikes": 36000,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "Mercola",
	"siteCategory": "junk science",
	"siteUrl": "http://www.mercola.com/",
	"siteGoogleHits": 4500000,
	"siteFacebookLikes": 1482835,
	"siteTwitterFollowers": 248000,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Modern Liberals",
	"siteCategory": "clickbait",
	"siteUrl": "http://modernliberals.com/",
	"siteGoogleHits": 96300,
	"siteFacebookLikes": 54511,
	"siteTwitterFollowers": 97,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Molon Labe Media",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.molonlabemedia.com/",
	"siteGoogleHits": 9250,
	"siteFacebookLikes": 11839,
	"siteTwitterFollowers": 193,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Morning Ledger",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.morningledger.com/",
	"siteGoogleHits": 258000,
	"siteFacebookLikes": 34303,
	"siteTwitterFollowers": 57,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Morning News USA",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.morningnewsusa.com/",
	"siteGoogleHits": 244000,
	"siteFacebookLikes": 8774,
	"siteTwitterFollowers": 5703,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "Move On",
	"siteCategory": "clickbait",
	"siteUrl": "http://front.moveon.org/",
	"siteGoogleHits": 25100000,
	"siteFacebookLikes": 1013838,
	"siteTwitterFollowers": 191155,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "MyZoneToday",
	"siteCategory": "clickbait",
	"siteUrl": "http://myzonetoday.com/",
	"siteGoogleHits": 3560,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "NahaDaily",
	"siteCategory": "satire",
	"siteUrl": "https://www.facebook.com/NahaDaily/",
	"siteGoogleHits": 7090,
	"siteFacebookLikes": 2371,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Nation of Change",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.nationofchange.org/",
	"siteGoogleHits": 352000,
	"siteFacebookLikes": 102838,
	"siteTwitterFollowers": 11300,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "National Policy Institute",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.npiamerica.org/",
	"siteGoogleHits": 244000,
	"siteFacebookLikes": 3798,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "National Report",
	"siteCategory": "satire",
	"siteUrl": "http://nationalreport.net/",
	"siteGoogleHits": 1500000,
	"siteFacebookLikes": 28014,
	"siteTwitterFollowers": 4139,
	"sitePoliticalAlignment": "centrist",
	"siteNotes": ""
}, {
	"siteTitle": "National Review",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.nationalreview.com/",
	"siteGoogleHits": 3750000,
	"siteFacebookLikes": 1034538,
	"siteTwitterFollowers": 205000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "National Rifle Association (NRA)",
	"siteCategory": "clickbait",
	"siteUrl": "https://home.nra.org/",
	"siteGoogleHits": 2170000,
	"siteFacebookLikes": 5087364,
	"siteTwitterFollowers": 413000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Natural Cures Not Medicine",
	"siteCategory": "junk science",
	"siteUrl": "https://www.facebook.com/NaturalCuresNotMedicine/",
	"siteGoogleHits": 662000,
	"siteFacebookLikes": 2060645,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "NaturalNews.com",
	"siteCategory": "junk science",
	"siteUrl": "http://www.naturalnews.com/",
	"siteGoogleHits": 2400000,
	"siteFacebookLikes": 2046926,
	"siteTwitterFollowers": 109000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "NC Scooper",
	"siteCategory": "satire",
	"siteUrl": "https://www.ncscooper.com/",
	"siteGoogleHits": 16100,
	"siteFacebookLikes": 41312,
	"siteTwitterFollowers": 3417,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "NCT (New Century Times)",
	"siteCategory": "clickbait",
	"siteUrl": "http://newcenturytimes.com/",
	"siteGoogleHits": 37200,
	"siteFacebookLikes": 1176345,
	"siteTwitterFollowers": 14800,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Nevo News",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.nevo.news/",
	"siteGoogleHits": 2340000,
	"siteFacebookLikes": 145100,
	"siteTwitterFollowers": 38,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "New Left Review",
	"siteCategory": "clickbait",
	"siteUrl": "https://newleftreview.org/",
	"siteGoogleHits": 486000,
	"siteFacebookLikes": 47105,
	"siteTwitterFollowers": 24300,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "New Republic",
	"siteCategory": "clickbait",
	"siteUrl": "https://newrepublic.com/",
	"siteGoogleHits": 5480000,
	"siteFacebookLikes": 156870,
	"siteTwitterFollowers": 150000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "News Corpse",
	"siteCategory": "clickbait",
	"siteUrl": "http://newscorpse.com/",
	"siteGoogleHits": 2649301,
	"siteFacebookLikes": 17163,
	"siteTwitterFollowers": 1746,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "News Examiner",
	"siteCategory": "clickbait",
	"siteUrl": "newsexaminer.net",
	"siteGoogleHits": 128000,
	"siteFacebookLikes": 344,
	"siteTwitterFollowers": 9,
	"sitePoliticalAlignment": "centrist",
	"siteNotes": "allegedly mixed to circumvent FB crackdown on fake news"
}, {
	"siteTitle": "News With Views",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.newswithviews.com/",
	"siteGoogleHits": 137000,
	"siteFacebookLikes": 3280,
	"siteTwitterFollowers": 619,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "News10Live",
	"siteCategory": "fake news",
	"siteUrl": "http://news10live.com/",
	"siteGoogleHits": 77700,
	"siteFacebookLikes": 2585,
	"siteTwitterFollowers": 149000,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "NewsBiscuit",
	"siteCategory": "satire",
	"siteUrl": "http://www.newsbiscuit.com/",
	"siteGoogleHits": 49600,
	"siteFacebookLikes": 9112,
	"siteTwitterFollowers": 12700,
	"sitePoliticalAlignment": "centrist",
	"siteNotes": ""
}, {
	"siteTitle": "Newsbusters",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.newsbusters.org/",
	"siteGoogleHits": 1260000,
	"siteFacebookLikes": 2649301,
	"siteTwitterFollowers": 162000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "NewsBuzzDaily",
	"siteCategory": "satire",
	"siteUrl": "https://www.facebook.com/NewsBuzzDaily",
	"siteGoogleHits": 2530,
	"siteFacebookLikes": 4677,
	"siteTwitterFollowers": 175,
	"sitePoliticalAlignment": "",
	"siteNotes": "They state: 'a combination of real shocking news and satire news'"
}, {
	"siteTitle": "NewsHounds",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.newshounds.us/",
	"siteGoogleHits": 254000,
	"siteFacebookLikes": 2955,
	"siteTwitterFollowers": 2300,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Newslo",
	"siteCategory": "satire",
	"siteUrl": "http://politicops.com/about-us/",
	"siteGoogleHits": 373000,
	"siteFacebookLikes": 180128,
	"siteTwitterFollowers": 19700,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "Newsmax",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.newsmax.com/",
	"siteGoogleHits": 10700000,
	"siteFacebookLikes": 1158815,
	"siteTwitterFollowers": 64100,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "NewsMutiny",
	"siteCategory": "satire",
	"siteUrl": "http://newsmutiny.com/",
	"siteGoogleHits": 6730,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "NewsWatch33 (formerly Newswatch28)",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.facebook.com/newswatch33/",
	"siteGoogleHits": 149000,
	"siteFacebookLikes": 460660,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": "allegedly mixed to circumvent FB crackdown on fake news"
}, {
	"siteTitle": "Next News Network",
	"siteCategory": "clickbait",
	"siteUrl": "http://nextnewsnetwork.com/",
	"siteGoogleHits": 352000,
	"siteFacebookLikes": 10387,
	"siteTwitterFollowers": 5284,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "NoDisInfo",
	"siteCategory": "conspiracy",
	"siteUrl": "http://nodisinfo.com/",
	"siteGoogleHits": 47600,
	"siteFacebookLikes": 249,
	"siteTwitterFollowers": 1335,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Nos Comunicamos",
	"siteCategory": "clickbait",
	"siteUrl": "http://noscomunicamos.com/",
	"siteGoogleHits": 1550000,
	"siteFacebookLikes": 16514,
	"siteTwitterFollowers": 783,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Now8News",
	"siteCategory": "fake news",
	"siteUrl": "http://now8news.com/",
	"siteGoogleHits": 81900,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 159000,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "NowTheEndBegins",
	"siteCategory": "satire",
	"siteUrl": "http://www.nowtheendbegins.com/",
	"siteGoogleHits": 180000,
	"siteFacebookLikes": 143782,
	"siteTwitterFollowers": 12100,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "NowThis News",
	"siteCategory": "clickbait",
	"siteUrl": "https://nowthisnews.com/",
	"siteGoogleHits": 411000,
	"siteFacebookLikes": 8540725,
	"siteTwitterFollowers": 451000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Occupy Democrats",
	"siteCategory": "clickbait",
	"siteUrl": "http://occupydemocrats.com/",
	"siteGoogleHits": 1960000,
	"siteFacebookLikes": 4650122,
	"siteTwitterFollowers": 18800,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "One America News Network",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.oann.com/",
	"siteGoogleHits": 188000,
	"siteFacebookLikes": 113021,
	"siteTwitterFollowers": 50100,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Online Conservative Press",
	"siteCategory": "conspiracy",
	"siteUrl": "http://onlineconservativepress.com/",
	"siteGoogleHits": 48800000,
	"siteFacebookLikes": 162617,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Opposing Views",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.opposingviews.com/",
	"siteGoogleHits": 4200000,
	"siteFacebookLikes": 3765123,
	"siteTwitterFollowers": 38500,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Pak Alert Press",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.pakalertpress.com/",
	"siteGoogleHits": 97300,
	"siteFacebookLikes": 87817,
	"siteTwitterFollowers": 9057,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Patriot Update",
	"siteCategory": "conspiracy",
	"siteUrl": "http://patriotupdate.com/",
	"siteGoogleHits": 489000,
	"siteFacebookLikes": 271863,
	"siteTwitterFollowers": 21600,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Personal Liberty",
	"siteCategory": "clickbait",
	"siteUrl": "http://personalliberty.com/",
	"siteGoogleHits": 1700000,
	"siteFacebookLikes": 1200000,
	"siteTwitterFollowers": 4600,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "PJ Media",
	"siteCategory": "clickbait",
	"siteUrl": "https://pjmedia.com/",
	"siteGoogleHits": 784000,
	"siteFacebookLikes": 349000,
	"siteTwitterFollowers": 50200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "PM Nightly News",
	"siteCategory": "clickbait",
	"siteUrl": "http://pmnightlynews.com/",
	"siteGoogleHits": 10600,
	"siteFacebookLikes": 5622,
	"siteTwitterFollowers": 1385,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Policy Review",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.policyreview.eu/",
	"siteGoogleHits": 3590000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 204,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Political Ears",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.politicalears.com/",
	"siteGoogleHits": 20600,
	"siteFacebookLikes": 770000,
	"siteTwitterFollowers": 25,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Political Insider",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.thepoliticalinsider.com/",
	"siteGoogleHits": 1280000,
	"siteFacebookLikes": 2753210,
	"siteTwitterFollowers": 30700,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Political Updater",
	"siteCategory": "clickbait",
	"siteUrl": "http://politicalupdater.com/",
	"siteGoogleHits": 801,
	"siteFacebookLikes": 998097,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "PoliticalBlindSpot",
	"siteCategory": "clickbait",
	"siteUrl": "http://politicalblindspot.com/",
	"siteGoogleHits": 31300,
	"siteFacebookLikes": 24658,
	"siteTwitterFollowers": 903,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Politichicks",
	"siteCategory": "clickbait",
	"siteUrl": "http://politichicks.com/",
	"siteGoogleHits": 128000,
	"siteFacebookLikes": 149131,
	"siteTwitterFollowers": 17300,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "PoliticusUSA",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.politicususa.com/",
	"siteGoogleHits": 705000,
	"siteFacebookLikes": 648216,
	"siteTwitterFollowers": 50600,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Power Line",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.powerlineblog.com/",
	"siteGoogleHits": 20400000,
	"siteFacebookLikes": 9863,
	"siteTwitterFollowers": 6890,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Pravda Report",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.pravdareport.com/",
	"siteGoogleHits": 229000,
	"siteFacebookLikes": 63619,
	"siteTwitterFollowers": 20400,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "PrisonPlanet.com",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.prisonplanet.com/",
	"siteGoogleHits": 1210000,
	"siteFacebookLikes": 23371,
	"siteTwitterFollowers": 378000,
	"sitePoliticalAlignment": "",
	"siteNotes": "Alex Jones network"
}, {
	"siteTitle": "Prntly",
	"siteCategory": "clickbait",
	"siteUrl": "http://prntly.com/",
	"siteGoogleHits": 39900,
	"siteFacebookLikes": 92349,
	"siteTwitterFollowers": 726,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Pro-America News",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.proamericanews.com/",
	"siteGoogleHits": 553000,
	"siteFacebookLikes": 297437,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Progressives Today",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.progressivestoday.com/",
	"siteGoogleHits": 61100,
	"siteFacebookLikes": 2618,
	"siteTwitterFollowers": 10000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "ProjectVeritas",
	"siteCategory": "clickbait",
	"siteUrl": "http://projectveritas.com/",
	"siteGoogleHits": 4590000,
	"siteFacebookLikes": 128633,
	"siteTwitterFollowers": 83500,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Prophecy Today",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.prophecytoday.com/",
	"siteGoogleHits": 80500,
	"siteFacebookLikes": 11343,
	"siteTwitterFollowers": 1908,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Proud Conservative",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.proudcons.com/",
	"siteGoogleHits": 251000,
	"siteFacebookLikes": 655689,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Proud Democrat",
	"siteCategory": "clickbait",
	"siteUrl": "http://proudemocrat.com/",
	"siteGoogleHits": 17800000,
	"siteFacebookLikes": 545470,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Raw Story",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.rawstory.com/",
	"siteGoogleHits": 1580000,
	"siteFacebookLikes": 758151,
	"siteTwitterFollowers": 109000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "React 365",
	"siteCategory": "fake news",
	"siteUrl": "http://www.react365.com/",
	"siteGoogleHits": 16200,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "none",
	"siteNotes": "Generate your own fake news"
}, {
	"siteTitle": "Reagan Coalition",
	"siteCategory": "clickbait",
	"siteUrl": "http://reagancoalition.com/",
	"siteGoogleHits": 111000,
	"siteFacebookLikes": 253388,
	"siteTwitterFollowers": 44700,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Real Time Politics",
	"siteCategory": "clickbait",
	"siteUrl": "http://realtimepolitics.com/",
	"siteGoogleHits": 51400,
	"siteFacebookLikes": 998200,
	"siteTwitterFollowers": 83100,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "RealFarmacy",
	"siteCategory": "junk science",
	"siteUrl": "http://www.realfarmacy.com/",
	"siteGoogleHits": 671000,
	"siteFacebookLikes": 859946,
	"siteTwitterFollowers": 2278,
	"sitePoliticalAlignment": "none",
	"siteNotes": "Old news, opinion pieces, some inaccurate some not"
}, {
	"siteTitle": "RealNewsRightNow",
	"siteCategory": "satire",
	"siteUrl": "http://realnewsrightnow.com/",
	"siteGoogleHits": 11500,
	"siteFacebookLikes": 1559,
	"siteTwitterFollowers": 499,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "Red Flag News",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.redflagnews.com/",
	"siteGoogleHits": 393000,
	"siteFacebookLikes": 274221,
	"siteTwitterFollowers": 11100,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Red Pepper",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.redpepper.org.uk/",
	"siteGoogleHits": 21100000,
	"siteFacebookLikes": 12909,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Red State",
	"siteCategory": "",
	"siteUrl": "http://www.redstate.com/",
	"siteGoogleHits": 1330000,
	"siteFacebookLikes": 533264,
	"siteTwitterFollowers": 182000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Red State Watcher",
	"siteCategory": "clickbait",
	"siteUrl": "http://redstatewatcher.com/",
	"siteGoogleHits": 106000,
	"siteFacebookLikes": 533261,
	"siteTwitterFollowers": 568,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Reductress",
	"siteCategory": "satire",
	"siteUrl": "http://reductress.com/",
	"siteGoogleHits": 134000,
	"siteFacebookLikes": 109274,
	"siteTwitterFollowers": 66300,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "Regated News",
	"siteCategory": "clickbait",
	"siteUrl": "https://regated.com/",
	"siteGoogleHits": 768,
	"siteFacebookLikes": 960,
	"siteTwitterFollowers": 16500,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Rense",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.rense.com/",
	"siteGoogleHits": 4030000,
	"siteFacebookLikes": 316,
	"siteTwitterFollowers": 260,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Reverb Press",
	"siteCategory": "clickbait",
	"siteUrl": "http://reverbpress.com/",
	"siteGoogleHits": 268000,
	"siteFacebookLikes": 638740,
	"siteTwitterFollowers": 16500,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Revolution News",
	"siteCategory": "clickbait",
	"siteUrl": "http://revnews.tumblr.com/",
	"siteGoogleHits": 537000,
	"siteFacebookLikes": 1092256,
	"siteTwitterFollowers": 46000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Rewire",
	"siteCategory": "clickbait",
	"siteUrl": "https://rewire.news/",
	"siteGoogleHits": 4010000,
	"siteFacebookLikes": 15000,
	"siteTwitterFollowers": 255,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Right Wing News",
	"siteCategory": "clickbait",
	"siteUrl": "http://rightwingnews.com/",
	"siteGoogleHits": 808000,
	"siteFacebookLikes": 3420732,
	"siteTwitterFollowers": 112000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Right Wing Watch",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.rightwingwatch.org/",
	"siteGoogleHits": 343000,
	"siteFacebookLikes": 135336,
	"siteTwitterFollowers": 45000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "RileNews",
	"siteCategory": "satire",
	"siteUrl": "http://www.rilenews.com/",
	"siteGoogleHits": 1390,
	"siteFacebookLikes": 370,
	"siteTwitterFollowers": 7,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "Ring of Fire",
	"siteCategory": "clickbait",
	"siteUrl": "https://trofire.com/",
	"siteGoogleHits": 12000000,
	"siteFacebookLikes": 200356,
	"siteTwitterFollowers": 27400,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "RockCityTimes",
	"siteCategory": "satire",
	"siteUrl": "http://www.rockcitytimes.com/",
	"siteGoogleHits": 14600,
	"siteFacebookLikes": 13781,
	"siteTwitterFollowers": 3058,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Satira Tribune",
	"siteCategory": "fake news",
	"siteUrl": "http://www.satiratribune.com/",
	"siteGoogleHits": 11800,
	"siteFacebookLikes": 30418,
	"siteTwitterFollowers": 924,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "SCEPCOP (Debunking Skeptics)",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.debunkingskeptics.com/",
	"siteGoogleHits": 7690,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 30,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Secrets of the Fed",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.secretsofthefed.com/",
	"siteGoogleHits": 3530000,
	"siteFacebookLikes": 19832,
	"siteTwitterFollowers": 2944,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Shareblue",
	"siteCategory": "clickbait",
	"siteUrl": "http://shareblue.com/",
	"siteGoogleHits": 399000,
	"siteFacebookLikes": 1037911,
	"siteTwitterFollowers": 23500,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Sheep Killers",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.sheepkillers.com/",
	"siteGoogleHits": 5180,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Shoebat",
	"siteCategory": "conspiracy",
	"siteUrl": "http://shoebat.com/",
	"siteGoogleHits": 545000,
	"siteFacebookLikes": 49000,
	"siteTwitterFollowers": 28700,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Silence is Consent",
	"siteCategory": "clickbait",
	"siteUrl": "http://silenceisconsent.net/",
	"siteGoogleHits": 92400,
	"siteFacebookLikes": 581241,
	"siteTwitterFollowers": 2888,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Skeptiko",
	"siteCategory": "conspiracy",
	"siteUrl": "http://skeptiko.com/",
	"siteGoogleHits": 60600,
	"siteFacebookLikes": 3361,
	"siteTwitterFollowers": 1304,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Socialist Standard",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.worldsocialism.org",
	"siteGoogleHits": 44200,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "SourceWatch",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.sourcewatch.org/",
	"siteGoogleHits": 2230000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 625,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "South Front",
	"siteCategory": "conspiracy",
	"siteUrl": "https://southfront.org/",
	"siteGoogleHits": 1620000,
	"siteFacebookLikes": 42388,
	"siteTwitterFollowers": 7359,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Storm Clouds Gathering",
	"siteCategory": "conspiracy",
	"siteUrl": "http://stormcloudsgathering.com/",
	"siteGoogleHits": 309000,
	"siteFacebookLikes": 320227,
	"siteTwitterFollowers": 27100,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Supreme Patriot",
	"siteCategory": "clickbait",
	"siteUrl": "http://supremepatriot.com/",
	"siteGoogleHits": 149000,
	"siteFacebookLikes": 598953,
	"siteTwitterFollowers": 53,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Sure News",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.surenews.com/",
	"siteGoogleHits": 96000,
	"siteFacebookLikes": 56418,
	"siteTwitterFollowers": 136,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Sustainable Pulse",
	"siteCategory": "conspiracy",
	"siteUrl": "http://sustainablepulse.com/",
	"siteGoogleHits": 52900,
	"siteFacebookLikes": 28010,
	"siteTwitterFollowers": 2769,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "TakePart",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.takepart.com/",
	"siteGoogleHits": 80000000,
	"siteFacebookLikes": 681116,
	"siteTwitterFollowers": 96500,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Talking Points Memo",
	"siteCategory": "clickbait",
	"siteUrl": "http://talkingpointsmemo.com/",
	"siteGoogleHits": 1660000,
	"siteFacebookLikes": 408279,
	"siteTwitterFollowers": 230000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "TD Newswire",
	"siteCategory": "clickbait",
	"siteUrl": "http://tdnewswire.com/",
	"siteGoogleHits": 399000,
	"siteFacebookLikes": 126710,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Tea Party News (TPNN)",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.westernjournalism.com/thepoint/",
	"siteGoogleHits": 181000,
	"siteFacebookLikes": 1368926,
	"siteTwitterFollowers": 20100,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Tea Party Tribune",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.teapartytribune.com/",
	"siteGoogleHits": 54400,
	"siteFacebookLikes": 14282,
	"siteTwitterFollowers": 3448,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Tell Me Now",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.tmn.today/?source=tellmenow.com",
	"siteGoogleHits": 1250000,
	"siteFacebookLikes": 2252870,
	"siteTwitterFollowers": 1900,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Advocate",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.advocate.com/",
	"siteGoogleHits": 906000,
	"siteFacebookLikes": 443630,
	"siteTwitterFollowers": 217000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The American Cause",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.theamericancause.org/",
	"siteGoogleHits": 164000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 29,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The American Conservative",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.theamericanconservative.com/",
	"siteGoogleHits": 69900000,
	"siteFacebookLikes": 52069,
	"siteTwitterFollowers": 21200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The American Mirror",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.theamericanmirror.com/",
	"siteGoogleHits": 191000,
	"siteFacebookLikes": 117976,
	"siteTwitterFollowers": 4585,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The American Prospect",
	"siteCategory": "clickbait",
	"siteUrl": "http://prospect.org/",
	"siteGoogleHits": 384000,
	"siteFacebookLikes": 108450,
	"siteTwitterFollowers": 26400,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The Angry Patriot",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.angrypatriotmovement.com/",
	"siteGoogleHits": 379000,
	"siteFacebookLikes": 1096662,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Anti-Media",
	"siteCategory": "conspiracy",
	"siteUrl": "http://theantimedia.org/",
	"siteGoogleHits": 222000,
	"siteFacebookLikes": 1948859,
	"siteTwitterFollowers": 39200,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Blacksphere",
	"siteCategory": "clickbait",
	"siteUrl": "http://theblacksphere.net/",
	"siteGoogleHits": 193000,
	"siteFacebookLikes": 523125,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Blaze",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.theblaze.com/",
	"siteGoogleHits": 3120000,
	"siteFacebookLikes": 1958324,
	"siteTwitterFollowers": 581000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Blue Route",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.blue-route.org/blog/",
	"siteGoogleHits": 546000,
	"siteFacebookLikes": 21086,
	"siteTwitterFollowers": 1002,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The Boston Tribune",
	"siteCategory": "clickbait",
	"siteUrl": "http://thebostontribune.com/",
	"siteGoogleHits": 16000000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 204,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Common Sense Show",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.thecommonsenseshow.com/",
	"siteGoogleHits": 171000,
	"siteFacebookLikes": 5604,
	"siteTwitterFollowers": 2171,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Constitution",
	"siteCategory": "clickbait",
	"siteUrl": "http://constitution.com/",
	"siteGoogleHits": 182000000,
	"siteFacebookLikes": 948593,
	"siteTwitterFollowers": 2193,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Controversial Files",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.thecontroversialfiles.net/",
	"siteGoogleHits": 4380000,
	"siteFacebookLikes": 310792,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The D.C. Clothesline",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.dcclothesline.com/",
	"siteGoogleHits": 80400,
	"siteFacebookLikes": 108345,
	"siteTwitterFollowers": 13900,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Daily Banter",
	"siteCategory": "clickbait",
	"siteUrl": "http://thedailybanter.com/",
	"siteGoogleHits": 81700,
	"siteFacebookLikes": 25139,
	"siteTwitterFollowers": 5417,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The Daily Sheeple",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.thedailysheeple.com/",
	"siteGoogleHits": 250000,
	"siteFacebookLikes": 56079,
	"siteTwitterFollowers": 8319,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Daily Wire",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.dailywire.com/",
	"siteGoogleHits": 25200,
	"siteFacebookLikes": 1388359,
	"siteTwitterFollowers": 21800,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The European Union Times",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.eutimes.net/",
	"siteGoogleHits": 129000000,
	"siteFacebookLikes": 348,
	"siteTwitterFollowers": 988,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Event Chronicle",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.theeventchronicle.com/#",
	"siteGoogleHits": 117000,
	"siteFacebookLikes": 60352,
	"siteTwitterFollowers": 2983,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Federalist",
	"siteCategory": "clickbait",
	"siteUrl": "http://thefederalist.com/",
	"siteGoogleHits": 4040000,
	"siteFacebookLikes": 45518,
	"siteTwitterFollowers": 49200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Federalist Papers Project",
	"siteCategory": "clickbait",
	"siteUrl": "http://thefederalistpapers.org/about",
	"siteGoogleHits": 522000,
	"siteFacebookLikes": 2237993,
	"siteTwitterFollowers": 7133,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Federation for American Immigration Reform",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.fairus.org/",
	"siteGoogleHits": 1150000,
	"siteFacebookLikes": 1127555,
	"siteTwitterFollowers": 72700,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Forbidden Knowledge",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.theforbiddenknowledge.com/",
	"siteGoogleHits": 993000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Gateway Pundit",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.thegatewaypundit.com/",
	"siteGoogleHits": 670000,
	"siteFacebookLikes": 585736,
	"siteTwitterFollowers": 60700,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Last Great Stand",
	"siteCategory": "conspiracy",
	"siteUrl": "https://thelastgreatstand.com/",
	"siteGoogleHits": 237000000,
	"siteFacebookLikes": 119303,
	"siteTwitterFollowers": 72600,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Liberty Beacon",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.thelibertybeacon.com/",
	"siteGoogleHits": 50300,
	"siteFacebookLikes": 22578,
	"siteTwitterFollowers": 222,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Mind Unleashed",
	"siteCategory": "conspiracy",
	"siteUrl": "http://themindunleashed.com/",
	"siteGoogleHits": 977000,
	"siteFacebookLikes": 7843017,
	"siteTwitterFollowers": 13000,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Morning Star",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.morningstaronline.co.uk/",
	"siteGoogleHits": 5250000,
	"siteFacebookLikes": 10988,
	"siteTwitterFollowers": 32000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The New Civil Rights Movement",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.thenewcivilrightsmovement.com/",
	"siteGoogleHits": 31000000,
	"siteFacebookLikes": 369974,
	"siteTwitterFollowers": 7135,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The Onion",
	"siteCategory": "satire",
	"siteUrl": "http://www.theonion.com/",
	"siteGoogleHits": 3300000,
	"siteFacebookLikes": 6134195,
	"siteTwitterFollowers": 9210000,
	"sitePoliticalAlignment": "centrist",
	"siteNotes": ""
}, {
	"siteTitle": "The Other 98%",
	"siteCategory": "clickbait",
	"siteUrl": "http://other98.com/",
	"siteGoogleHits": 3900,
	"siteFacebookLikes": 3583520,
	"siteTwitterFollowers": 13900,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The Patriot Post",
	"siteCategory": "clickbait",
	"siteUrl": "https://patriotpost.us/",
	"siteGoogleHits": 198000,
	"siteFacebookLikes": 518534,
	"siteTwitterFollowers": 5895,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Post and Mail",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.thepostandmail.com/",
	"siteGoogleHits": 266000,
	"siteFacebookLikes": 4949,
	"siteTwitterFollowers": 719,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Progressive",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.progressive.org/",
	"siteGoogleHits": 19100000,
	"siteFacebookLikes": 38410,
	"siteTwitterFollowers": 29400,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The Real Strategy",
	"siteCategory": "clickbait",
	"siteUrl": "https://therealstrategy.com/",
	"siteGoogleHits": 92800,
	"siteFacebookLikes": 8700,
	"siteTwitterFollowers": 2798,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Rebel",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.therebel.media/",
	"siteGoogleHits": 16100000,
	"siteFacebookLikes": 56902,
	"siteTwitterFollowers": 44200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Right Scoop",
	"siteCategory": "clickbait",
	"siteUrl": "http://therightscoop.com/",
	"siteGoogleHits": 209000,
	"siteFacebookLikes": 98533,
	"siteTwitterFollowers": 14300,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Root",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.theroot.com/",
	"siteGoogleHits": 66700000,
	"siteFacebookLikes": 889604,
	"siteTwitterFollowers": 288000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "The Rundown Live",
	"siteCategory": "conspiracy",
	"siteUrl": "http://therundownlive.com/",
	"siteGoogleHits": 44700,
	"siteFacebookLikes": 19226,
	"siteTwitterFollowers": 2519,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The Stately Harold",
	"siteCategory": "satire",
	"siteUrl": "http://vindoga.wixsite.com/thestatelyharold",
	"siteGoogleHits": 2890,
	"siteFacebookLikes": 1890,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "The Truth About Cancer",
	"siteCategory": "junk science",
	"siteUrl": "https://thetruthaboutcancer.com/",
	"siteGoogleHits": 513000,
	"siteFacebookLikes": 775430,
	"siteTwitterFollowers": 4092,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Truth Seeker",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.thetruthseeker.co.uk/",
	"siteGoogleHits": 609000,
	"siteFacebookLikes": 34611,
	"siteTwitterFollowers": 81900,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "The US Patriot",
	"siteCategory": "clickbait",
	"siteUrl": "http://theuspatriot.com/",
	"siteGoogleHits": 147000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "The Walrus",
	"siteCategory": "clickbait",
	"siteUrl": "https://thewalrus.ca/",
	"siteGoogleHits": 2840000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 69200,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "TheGrio",
	"siteCategory": "clickbait",
	"siteUrl": "http://thegrio.com/",
	"siteGoogleHits": 733000,
	"siteFacebookLikes": 970095,
	"siteTwitterFollowers": 73100,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "TheLapine.ca",
	"siteCategory": "satire",
	"siteUrl": "https://thelapine.ca/",
	"siteGoogleHits": 23300,
	"siteFacebookLikes": 5275,
	"siteTwitterFollowers": 983,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "TheNewEuropean",
	"siteCategory": "",
	"siteUrl": "http://www.theneweuropean.co.uk/home",
	"siteGoogleHits": 488000,
	"siteFacebookLikes": 7520,
	"siteTwitterFollowers": 16400,
	"sitePoliticalAlignment": "centre/left??",
	"siteNotes": ""
}, {
	"siteTitle": "TheNewsNerd",
	"siteCategory": "fake news",
	"siteUrl": "http://www.thenewsnerd.com/",
	"siteGoogleHits": 12800,
	"siteFacebookLikes": 5615,
	"siteTwitterFollowers": 209,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "TheSpoof",
	"siteCategory": "satire",
	"siteUrl": "http://www.thespoof.com/",
	"siteGoogleHits": 487000,
	"siteFacebookLikes": 358,
	"siteTwitterFollowers": 754,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "TheUsPatriot.com",
	"siteCategory": "conspiracy",
	"siteUrl": "http://theuspatriot.com/",
	"siteGoogleHits": 25900,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": "Realorsatire.com concludes: theuspatriot.com is full of anti-Obama, anti-progress, anti-Left, anti-Democrat non-news, that either they are being satirical, or they are just being assholes who are pushing wholly incorrect — and already disproved — information."
}, {
	"siteTitle": "Think Progress",
	"siteCategory": "clickbait",
	"siteUrl": "https://thinkprogress.org/",
	"siteGoogleHits": 1870000,
	"siteFacebookLikes": 1759622,
	"siteTwitterFollowers": 647000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Thrive Movement",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.thrivemovement.com/",
	"siteGoogleHits": 301000,
	"siteFacebookLikes": 303588,
	"siteTwitterFollowers": 25800,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "TMZ WorldNews",
	"siteCategory": "satire",
	"siteUrl": "http://tmzworldnews.com/",
	"siteGoogleHits": 96900,
	"siteFacebookLikes": 344543,
	"siteTwitterFollowers": 33829,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Topinfo Post",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.topinfopost.com/",
	"siteGoogleHits": 60100,
	"siteFacebookLikes": 38663,
	"siteTwitterFollowers": 5013,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Townhall",
	"siteCategory": "clickbait",
	"siteUrl": "http://townhall.com/",
	"siteGoogleHits": 18600000,
	"siteFacebookLikes": 1274178,
	"siteTwitterFollowers": 91200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Tribune UK",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.tribunemagazine.org/",
	"siteGoogleHits": 16300000,
	"siteFacebookLikes": 1985,
	"siteTwitterFollowers": 4757,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "True Activist",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.trueactivist.com/",
	"siteGoogleHits": 625000,
	"siteFacebookLikes": 1361960,
	"siteTwitterFollowers": 23200,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "True Pundit",
	"siteCategory": "conspiracy",
	"siteUrl": "http://truepundit.com/",
	"siteGoogleHits": 75300,
	"siteFacebookLikes": 1379,
	"siteTwitterFollowers": 24400,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Truth and Action",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.truthandaction.org/",
	"siteGoogleHits": 520000,
	"siteFacebookLikes": 790511,
	"siteTwitterFollowers": 46,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Truth Broadcasting Network",
	"siteCategory": "conspiracy",
	"siteUrl": "http://truthbroadcastnetwork.com/",
	"siteGoogleHits": 1970000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Truth In Media",
	"siteCategory": "clickbait",
	"siteUrl": "http://truthinmedia.com/",
	"siteGoogleHits": 296000,
	"siteFacebookLikes": 342292,
	"siteTwitterFollowers": 62300,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Truth Out",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.truth-out.org/",
	"siteGoogleHits": 748000,
	"siteFacebookLikes": 748166,
	"siteTwitterFollowers": 146000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Truth Revolt",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.truthrevolt.org/",
	"siteGoogleHits": 297000,
	"siteFacebookLikes": 37068,
	"siteTwitterFollowers": 9667,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Truthdig",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.truthdig.com/",
	"siteGoogleHits": 569000,
	"siteFacebookLikes": 226911,
	"siteTwitterFollowers": 64900,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "TruthFeed",
	"siteCategory": "clickbait",
	"siteUrl": "http://truthfeed.com/",
	"siteGoogleHits": 302000,
	"siteFacebookLikes": 358975,
	"siteTwitterFollowers": 10600,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "TruthFrequencyRadio",
	"siteCategory": "conspiracy",
	"siteUrl": "http://truthfrequencyradio.com/",
	"siteGoogleHits": 88000,
	"siteFacebookLikes": 8048,
	"siteTwitterFollowers": 516,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "Twitchy",
	"siteCategory": "clickbait",
	"siteUrl": "http://twitchy.com/",
	"siteGoogleHits": 4560000,
	"siteFacebookLikes": 1277992,
	"siteTwitterFollowers": 215000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "U.S. Chronicle",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.uschronicle.com/about-us/",
	"siteGoogleHits": 134000,
	"siteFacebookLikes": 357,
	"siteTwitterFollowers": 2,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "U.S. Herald",
	"siteCategory": "clickbait",
	"siteUrl": "http://usherald.com/",
	"siteGoogleHits": 67700,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 2516,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Uncle Sam’s Misguided Children",
	"siteCategory": "conspiracy",
	"siteUrl": "http://unclesamsmisguidedchildren.com/",
	"siteGoogleHits": 103000,
	"siteFacebookLikes": 23838,
	"siteTwitterFollowers": 15600,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "UnconfirmedSources",
	"siteCategory": "satire",
	"siteUrl": "http://unconfirmedsources.com/wp/",
	"siteGoogleHits": 689000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 90,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "Underground Health",
	"siteCategory": "junk science",
	"siteUrl": "https://www.undergroundhealth.com/",
	"siteGoogleHits": 165000,
	"siteFacebookLikes": 348276,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "UpliftConnect",
	"siteCategory": "junk science",
	"siteUrl": "spiritual",
	"siteGoogleHits": 366000,
	"siteFacebookLikes": 633386,
	"siteTwitterFollowers": 2267,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Uproxx",
	"siteCategory": "clickbait",
	"siteUrl": "http://uproxx.com/",
	"siteGoogleHits": 7080000,
	"siteFacebookLikes": 1782595,
	"siteTwitterFollowers": 74700,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "US Political Post",
	"siteCategory": "clickbait",
	"siteUrl": "http://uspoliticalpost.com/",
	"siteGoogleHits": 401,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "US Uncut",
	"siteCategory": "clickbait",
	"siteUrl": "http://usuncut.com/",
	"siteGoogleHits": 548000,
	"siteFacebookLikes": 1545799,
	"siteTwitterFollowers": 19000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "US.Blasting.News",
	"siteCategory": "clickbait",
	"siteUrl": "http://us.blastingnews.com/",
	"siteGoogleHits": 67800,
	"siteFacebookLikes": 49236,
	"siteTwitterFollowers": 2192,
	"sitePoliticalAlignment": "none",
	"siteNotes": ""
}, {
	"siteTitle": "USA Hitman",
	"siteCategory": "conspiracy",
	"siteUrl": "https://usahitman.com/",
	"siteGoogleHits": 38900,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 4629,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "USA Newsflash",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.usanewsflash.com/",
	"siteGoogleHits": 164000,
	"siteFacebookLikes": 646316,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "USA Politics Now",
	"siteCategory": "clickbait",
	"siteUrl": "http://usapoliticsnow.com/",
	"siteGoogleHits": 20400,
	"siteFacebookLikes": 5085,
	"siteTwitterFollowers": 104,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "USA Supreme",
	"siteCategory": "",
	"siteUrl": "-",
	"siteGoogleHits": 86500000,
	"siteFacebookLikes": 42633,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "VDARE",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.vdare.com/",
	"siteGoogleHits": 274000,
	"siteFacebookLikes": 9084,
	"siteTwitterFollowers": 22000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Veterans Today",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.veteranstoday.com/",
	"siteGoogleHits": 808000,
	"siteFacebookLikes": 41008,
	"siteTwitterFollowers": 32400,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Vidmax",
	"siteCategory": "clickbait",
	"siteUrl": "http://vidmax.com/",
	"siteGoogleHits": 360000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 799,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Viral Liberty",
	"siteCategory": "conspiracy",
	"siteUrl": "http://viralliberty.com/",
	"siteGoogleHits": 24500,
	"siteFacebookLikes": 96,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Washington Free Beacon",
	"siteCategory": "clickbait",
	"siteUrl": "http://freebeacon.com/",
	"siteGoogleHits": 3380000,
	"siteFacebookLikes": 720727,
	"siteTwitterFollowers": 67100,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Washington Monthly",
	"siteCategory": "clickbait",
	"siteUrl": "http://washingtonmonthly.com/",
	"siteGoogleHits": 447000,
	"siteFacebookLikes": 11366,
	"siteTwitterFollowers": 5510,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "We Are Change",
	"siteCategory": "conspiracy",
	"siteUrl": "http://wearechange.org/",
	"siteGoogleHits": 607000,
	"siteFacebookLikes": 449451,
	"siteTwitterFollowers": 55200,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Weasel Zippers",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.weaselzippers.us/",
	"siteGoogleHits": 11800,
	"siteFacebookLikes": 3613,
	"siteTwitterFollowers": 20200,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Web Daily",
	"siteCategory": "clickbait",
	"siteUrl": "https://www.webdaily.com/",
	"siteGoogleHits": 258000,
	"siteFacebookLikes": 3404128,
	"siteTwitterFollowers": 78,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Weekly Standard",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.weeklystandard.com/",
	"siteGoogleHits": 1090000,
	"siteFacebookLikes": 278820,
	"siteTwitterFollowers": 226000,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "WeeklyWorldNews.com",
	"siteCategory": "satire",
	"siteUrl": "http://weeklyworldnews.com/",
	"siteGoogleHits": 402000,
	"siteFacebookLikes": 103244,
	"siteTwitterFollowers": 2915,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Western Journalism",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.westernjournalism.com/",
	"siteGoogleHits": 1950000,
	"siteFacebookLikes": 4493372,
	"siteTwitterFollowers": 30700,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "WhatDoesItMean",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.whatdoesitmean.com/",
	"siteGoogleHits": 1540000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Why Don’t You Try This",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.whydontyoutrythis.com/",
	"siteGoogleHits": 108000,
	"siteFacebookLikes": 853482,
	"siteTwitterFollowers": null,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Winning Democrats",
	"siteCategory": "clickbait",
	"siteUrl": "http://winningdemocrats.com/",
	"siteGoogleHits": 528000,
	"siteFacebookLikes": 1207107,
	"siteTwitterFollowers": 44,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "WitScience",
	"siteCategory": "satire",
	"siteUrl": "http://witscience.org/",
	"siteGoogleHits": 13000,
	"siteFacebookLikes": 2918,
	"siteTwitterFollowers": 8,
	"sitePoliticalAlignment": "unknown",
	"siteNotes": ""
}, {
	"siteTitle": "WND (World Net Daily)",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.wnd.com/",
	"siteGoogleHits": 581000,
	"siteFacebookLikes": 824529,
	"siteTwitterFollowers": 63500,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Wonkette",
	"siteCategory": "clickbait",
	"siteUrl": "http://wonkette.com/",
	"siteGoogleHits": 551000,
	"siteFacebookLikes": null,
	"siteTwitterFollowers": 47000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "World News Daily Report",
	"siteCategory": "satire",
	"siteUrl": "http://worldnewsdailyreport.com/",
	"siteGoogleHits": 108000,
	"siteFacebookLikes": 27394,
	"siteTwitterFollowers": 95,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "World Truth TV",
	"siteCategory": "junk science",
	"siteUrl": "http://worldtruth.tv/",
	"siteGoogleHits": 431000,
	"siteFacebookLikes": 14162,
	"siteTwitterFollowers": 10800,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Young Conservatives",
	"siteCategory": "clickbait",
	"siteUrl": "http://www.youngcons.com/",
	"siteGoogleHits": 580000,
	"siteFacebookLikes": 813757,
	"siteTwitterFollowers": 85900,
	"sitePoliticalAlignment": "right",
	"siteNotes": ""
}, {
	"siteTitle": "Young Turks",
	"siteCategory": "clickbait",
	"siteUrl": "https://tytnetwork.com/",
	"siteGoogleHits": 8530000,
	"siteFacebookLikes": 1334954,
	"siteTwitterFollowers": 257000,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Your News Wire",
	"siteCategory": "conspiracy",
	"siteUrl": "http://yournewswire.com/",
	"siteGoogleHits": 315000,
	"siteFacebookLikes": 20619,
	"siteTwitterFollowers": 14600,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}, {
	"siteTitle": "Z Magazine",
	"siteCategory": "clickbait",
	"siteUrl": "https://zcomm.org/zmag/",
	"siteGoogleHits": 199000,
	"siteFacebookLikes": 855,
	"siteTwitterFollowers": 326,
	"sitePoliticalAlignment": "left",
	"siteNotes": ""
}, {
	"siteTitle": "Zero Hedge",
	"siteCategory": "conspiracy",
	"siteUrl": "http://www.zerohedge.com/",
	"siteGoogleHits": 2740000,
	"siteFacebookLikes": 14833,
	"siteTwitterFollowers": 373000,
	"sitePoliticalAlignment": "",
	"siteNotes": ""
}]
```
    



