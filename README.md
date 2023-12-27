## SEO Data Analytics Scripts
Currently using many different python script in order to answer very specific analytics questions. In this repo are my top ones - read some informations below.

### Top Query within Title / H1 Tag?
Had good success with updating / adding additional keywords from the top queries to title and / or h1 tag. The script does the following:
- Fetch current GSC data through google API
  - Generate top query for each landingpage in the date frame depending on clicks
- Join with current crawling data for each landingpage
- Calculate the Edit Distance between lists of strings using any distance/similarity based scorer (Link: https://maartengr.github.io/PolyFuzz/api/models/distance/)
- Add a threshold and filter for potential quick wins in Title Tag / H1, where the ranking of top query is worse than position 3
- Add / Update title tag / h1 tag with the top query and keep looking for ranking increases within the next couple of days

