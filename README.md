Data Science Blog Post
======================

This is my blog post for the data scientist nanodegree.  The code for
the data analysis is [`explore.py`](explore.py), and the report/blog
post is [here](blog.md).

The code uses the usual Python libraries, and requires the following
datasets:

* 2018 StackOverflow developer survey.  This can be downloaded
  [here](https://insights.stackoverflow.com/survey/); the zip file
  should be extracted in the `SODS2018` folder.

* OECD's gender pay gap data, available
  [here](https://data.oecd.org/earnwage/gender-wage-gap.htm), as file
  `gendergap.csv`.

* Exchange rates and PPP exchange rates, available
  [here](https://data.oecd.org/conversion/exchange-rates.htm) and
  [here](https://data.oecd.org/conversion/purchasing-power-parities-ppp.htm).

Moreover, median income data for a few countries is used.  The OECD
provides only median _disposable_ income information, which is not
meaningful in a comparison with the StackOverflow data.  Thus, I used
median income data from a Gallup poll, which can be seen [on
Wikipedia](https://en.wikipedia.org/wiki/Median_income).  This is not
available through an API, so I just copied the few required values
manually.
