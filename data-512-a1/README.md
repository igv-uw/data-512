# Objective
The objective of this repository is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from
January 1 2008 through August 30 2020, obtained from two public APIs.

# API information
The data combines information from two APIs.
- [Legacy Pagecounts API](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts): Provides access to desktop and mobile traffic data from December 2007 through July 2016.
- [Pageviews API](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews): Provides access to desktop, mobile web, and mobile app traffic data from July 2015 through last month.

# Generated Dataset Fields
| Column                  | Value         | Description                              |
|-------------------------|---------------|------------------------------------------|
| year                    | YYYY          | Year of observation                      |
| month                   | MM            | Month of observation                     |
| pagecount_all_views     | num_views     | Number of all views on Pagecount API     |
| pagecount_desktop_views | num_views     | Number of desktop views on Pagecount API |
| pagecount_mobile_views  | num_views     | Number of mobile views on Pagecount API  |
| pageview_all_views      | num_views     | Number of all views on Pageview API      |
| pageview_desktop_views  | num_views     | Number of desktop views on Pageview API  |
| pageview_mobile_views   | num_views     | Number of mobile views on Pageview API   |

# License and restrictions
- Project under [MIT License](LICENSE).  
- Data under Wikimedia [Terms of Use](https://foundation.wikimedia.org/wiki/Terms_of_Use/en).
- Wikimedia REST API terms of use at [Wikimedia Foundation](https://www.mediawiki.org/wiki/Wikimedia_REST_API#Terms_and_conditions).

# Issues and considerations
- Pageview API excludes spiders/crawlers, Pagecounts API does not.
- There is 1 year of data overlap between the APIs.
