### Goal of project
The goal of this project is to practice querying data using an open source API while maintaining good data science development practice.
A few analyses are done to further explore the number of view pages for the list of dinosaurs. During the process, best practices including clean code,
clear documentation and correct labelling of charts are being applied.

### License
MIT Open Source:https://opensource.org/licenses/MIT
Wikimedia Foundation REST API terms of use: https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions

### Link to API documentation
Wikimedia REST API documentation and reference: https://www.mediawiki.org/wiki/API:REST_API/Reference

### Files and data
- HW1.ipynb contains the script to collect, parse and analyse data.
- dino_monthly_mobile_201507_202209.json contains the number of view via mobile access.
- dino_monthly_desktop_201507_202209.json contains the number of view via desktop access.
- dino_monthly_cumulative_201507_202209.json contains the total number of view of mobile and desktop cumulative month over month.
- columns in the .json files: 
    - project: the type of Wikipedia page, in our case would be en.wikipedia
    - article: the dinosaur article that we will collect view from
    - granularity: the time period interested, in this case it is monthly
    - timestamp: the year and month of the view of the page
    - access: either mobile-web, mobile-app, desktop or all-access
    - agent: the type of user
    - views: the number of view of the Wikipedia article

