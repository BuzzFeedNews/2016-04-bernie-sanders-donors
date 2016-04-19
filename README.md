# Analysis of Bernie Sanders's ActBlue Donors

This repository contains data, code, and methodologies supporting the April 19, 2016 BuzzFeed News article, "[How Bernie Sanders Raises All That Money](http://www.buzzfeed.com/johntemplon/how-bernie-sanders-raises-all-that-money)."

- [Data](#data)
- [Analyses](#analyses)
- [Feedback](#feedback)

## Data

__ActBlue campaign finance filings.__  ActBlue, a political action committee, processes the vast majority of contributions to Bernie Sanders's 2016 presidential campaign. The analyses use ActBlue's `PRE-RUNOFF`, `POST-SPECIAL`, `PRE-PRIMARY`, `POST-RUN-OFF`, `MID-YEAR`, `YEAR-END`, `FEB MONTHLY`, and `MARCH MONTHLY` filings sent to the Federal Election Commission. These filings cover the entirety of the Sanders presidential campaign, which began on April 30, 2015. The data include all "receipts" for this time period, and were downloaded from ProPublica's [FEC Itemizer](https://projects.propublica.org/itemizer/committee/C00401224/2016). Some rows in the files contained unmatched quotation marks (e.g., `"NOT EMPLOYED,`) in the `employer` field. BuzzFeed News fixed those rows by hand; you can download these cleaned-up files [here](https://archive.org/details/actblue-fec-filings-april-2015-to-feb-2016).

__Census population figures.__ The Census Bureau reports population figures for geographies known as "[ZIP Code Tabulation Areas](https://www.census.gov/geo/reference/zctas.html)"; they don't overlap perfectly with ZIP codes, but they're as close as Census data gets. You can find the data in the `data/zcta-population` folder, which includes population and race totals from the 2010-2014 American Community Survey.

## Analyses

All analyses can be found in [this notebook](https://github.com/BuzzFeedNews/2016-04-bernie-sanders-donors/blob/master/notebooks/act-blue-analysis.ipynb). The methodologies and code there support the following passages from the BuzzFeed News article:

- "The huge spike in the middle of February came after Sanders raised $5.2 million in the 24 hours after he won the New Hampshire primary."

- "At least 29 Bernie donors have given at least 100 times through ActBlue, according to the data. They span the spectrum of Sanders’ base, from professionals to students. Among the 29 are a college student, an art historian, a lawyer, a pharmacist and a federal employee. Six of the 29 are from California. Five are from Texas."

- "53% of Sanders’ donors on ActBlue give just once (at an average donation of $33.) The vast majority of Sanders’ donors, 92%, donate less than $200."

- "The average overall of ActBlue donations is juuuust shy of the “twenty-seven dollars” Sanders talks about all the time. The real average is $26.87."

- "Crestone, Colorado has the highest concentration of Sanders donors by zip code per capita outside of Vermont. One hundred and seven of the 1,173 people who live in 81131 have donated to the Sanders campaign."

## Feedback?

Contact John Templon at [john.templon@buzzfeed.com](mailto:john.templon@buzzfeed.com).

Looking for more from BuzzFeed News? [Click here for a list of our open-sourced projects, data, and code](https://github.com/BuzzFeedNews/everything).
