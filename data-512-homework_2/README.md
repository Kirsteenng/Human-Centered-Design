### Goal of project
The goal of this project is to study the biases of the quality article on a list of politicians. The quality article of each article is retrieved 
using the ORES API. The following three aggregation analyses are done and the results are presented as table forms in the Jupyter notebook.
    - Top and bottom countries with article coverage per capita
    - Top and bottom countries with high quality article per capita
    - Top and bottom region with article coverage and high quality article per capita

### Data source
politician list:
population list:

### License
MIT Open Source:https://opensource.org/licenses/MIT
Wikimedia Foundation REST API terms of use: https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions
Creative Commons: https://creativecommons.org/share-your-work/public-domain/cc0/

### Link to API documentation
Wikimedia REST API documentation and reference: https://www.mediawiki.org/wiki/API:REST_API/Reference

### Files and data
- HW2.ipynb contains the script to collect, parse and analyse data.
- wp_countries-no_match.txt is one of the 
- wp_politicians_by_country.csv
- columns in the wp_politicians_by_country.csv files: 
    - country(str): the name of the country
    - region(str): the geographic region that the country belongs to
    - population(float): population of the country by millions
    - article_title(str): name of the politician in study
    - revision_id(int): id of the Wikipedia article retrieved using Wikimedia API
    - article_quality(str): quality of the Wikipedia article as predicted using ORES API
    

### Research Implications
## Expected biases from original dataset
Given the list of the politician is crawled from Wikipedia, it can be biased towards famous politicians and not a very representative list of 
all politicians from the world. Meanwhile, because Wikipedia is a crowd source based platform and given majority of the countries in the world are democratic 
and socialist countries, countries which do not conform to such political system might be left out from this list. It is expected that politicians from
communist based countries, such as Cuba or China, and countries which practice dictatorship, such as North Korea, will be limited or excluded.

## Initial bias discovered from data processing and analysis
After the first data exploration and analysis process, it is found that small and unpopular countries are representated with zero population.
At the same time, this group of countries do not have a lot of politicians available to them and hence users would think that these countries
do not produce important political figures. There are more politicians available in democratic, populous and growing countries such as France, India , Nigeria. Non english speaking countries, such as China, have limited politicians in the list. Small island nations, such as the Carribean islands, are well represented as well.

## Implication about (English) Wikipedia as a data source
Given the website is in English, the contributors have to be from the nations that are fluent in the language. This has introduced biased
in gettting the politician lists which serves as the starting point of this research. 
It is likely for people from non-English based countries to contribute articles in their most spoken language. 
An example would be Mexico. For such a populous and important country in North America, it is surprising to see there is only 1 politician from Mexico
on the list. Therefore this research should highlight the bias introduced since the beginning so that users are aware of the skewedness 
of the result and interpret them accordingly.

## Implication about the internet and global society in general
The quality and characteristic of open source platform such as Wikipedia is highly shaped by the majority of the contributors. 
Users and researchers have to be aware of the premise of the data collected at the beginning. For instance, in the case of this research
the original data is crawled from (English) Wikipedia and hence it will be biased towards countries that speak and have in-depth understanding
of English. At the same time, it is assumed that majority of the contributors also have more access to information about countries
that have democratic and socialist political system. Therefore, that would shape the quality of the articles which explains why the region of
Southern Europe, which countries have robust understanding of English and practice democracy political system,has the highest number of 
high quality articles.