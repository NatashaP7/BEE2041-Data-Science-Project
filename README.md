# BEE2041-Data-Science-Project 
## The Growth of K-Pop in the UK: Evidence from Concerts and Online Demand 
> Has K-pop gone mainstream in the UK? Tracing the growth of Korean live music from niche fandom to mainstream cultural presence, 2011–2025. 

--- 
## Project Overview 
This project analyses the growth of K-pop concerts in the United Kingdom between 2011 and 2025, using an original, hand-collected dataset of every K-pop concert in the UK during this period. It examines concert frequency, venue scale, geographic spread, and artist return rates to answer whether K-pop has crossed from niche fandom into mainstream live music culture. 

The analysis is enriched with two additional resources gathered through web scraping: venue capacities scraped from Wikipedia, and UK Google search interest for 'K-pop' retrieved via Google Trends. 

### Blog Post 
Read the full analysis here: [K-Pop Growth in the UK](https://hackmd.io/@__uw6hMvSWa_eMXtyExmLQ/rkNMBA3CWx)

**Module:** BEE2041 Data Science in Economics 
**Due Date:** 1st May 2026 (extension until 15th May 2026) 

## Project Structure 
```
BEE2041-Data-Science-Project/
│
├── README.md                        ← this file
├── kpop_concerts_in_the_uk.ipynb    ← main analysis notebook
├── data/
│   └── concert_data         ← hand-collected dataset of every K-pop concert in the UK from 2011 to 2027 (as │                               of April 2026)
│   └── concerts_main        ← concert dataset of only the years 2011-2025, including venues, and venue     │                                capacity  
├──output/
│   └── kpop_concerts_annual.png         ← bar chart of annual concerts held in the UK 2011-2027 
│   └── kpop_search_interest.png         ← line graph of UK Google search interest for 'K-pop' from 2011-2025
│   └── regression1_with_sensitivity.png         ← regression of search interest vs average venue capacity 
│   └── regression2_multiple.png         ← multiple regression of actual vs predicted concert count
│   └── kpop_geography.png         ← pie chart showing percentage of concerts held in London vs outside of   │                                     London and horizontal bar chart to show which cities these were 
│   └── repeat_artists.png         ← line graph showing the venue capacity of their concerts over the year 
└──────                               and bar chart to show geogrpahically where the concerts have been held 

```

## How to Replicate This Project 

### Requirements 
- Python 3.x (via Anaconda)
- Jupyter Notebook 

```
pip install pytrends pandas matplotlib seaborn statsmodels requests beautifulsoup4 scipy 
```

### Steps 
1. Clone or download this repository
2. Open `kpop_concerts_in_the_uk.ipynb` in Jupyter Notebook
3. Run all cells in order from top to bottom
4. The notebook will automatically scrape venue capacities from Wikipedia and retrieve Google Trends data (an internet connection is required)

### Data Sources 
- **Concert data:** Hand-collected by the author from sources including 
  Songkick, Setlist.fm, and fan community records (2011–2025, with partial data for 2026 and announced dates for 2027)
- **Venue capacities:** Scraped from Wikipedia using BeautifulSoup; 
  supplemented by a manual lookup table for smaller venues
- **Search interest:** UK Google Trends data for the keyword 'K-pop', 
  retrieved via the pytrends library

## Research Question
Has K-pop gone mainstream in the UK? This project traces the growth of 
Korean live music from its origins as a niche fandom activity in 2011 to 
the present day, examining what the data reveals about the genre's 
trajectory in the British music market.

## Tools Used
- Python (pandas, numpy, matplotlib, scipy)
- BeautifulSoup (web scraping)
- pytrends (Google Trends API)
- Jupyter Notebook
- Git / GitHub
