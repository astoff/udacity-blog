Data Science Blog Post
======================

This is my blog post for the data scientist nanodegree.  The code for
the data analysis is [`explore.ipynb`](explore.ipynb), and the
report/blog post is [here](blog.md).

Installation and fetching the data
----------------------------------

The code uses the usual Python libraries, and requires the following
datasets:

* 2018 StackOverflow developer survey.  This can be downloaded
  [here](https://insights.stackoverflow.com/survey/); the zip file
  should be extracted in the `SODS2018` folder.

* OECD's gender pay gap data, available
  [here](https://data.oecd.org/earnwage/gender-wage-gap.htm), as file
  `gendergap.csv`.  To get it, type
  ``` shell
  wget 'https://stats.oecd.org/sdmx-json/data/DP_LIVE/.WAGEGAP.../OECD?contentType=csv&detail=code&separator=comma&csv-lang=en' -O gendergap.csv
  ```

* Median income, exchange rates and PPP exchange rates, available
  [here](https://stats.oecd.org/Index.aspx?DataSetCode=IDD)
  [here](https://data.oecd.org/conversion/exchange-rates.htm) and
  [here](https://data.oecd.org/conversion/purchasing-power-parities-ppp.htm).
  ``` shell
  wget 'https://stats.oecd.org/sdmx-json/data/DP_LIVE/.EXCH.../OECD?contentType=csv&detail=code&separator=comma&csv-lang=en' -O exchange.csv
  wget 'https://stats.oecd.org/sdmx-json/data/DP_LIVE/.PPP.../OECD?contentType=csv&detail=code&separator=comma&csv-lang=en' -O ppp.csv
  ```

Moreover, median income data for a few countries is used.  The OECD
provides only median _disposable_ income information, which is not
meaningful in a comparison with the StackOverflow data.  Thus, I used
median income data from a Gallup poll, which can be seen [on
Wikipedia](https://en.wikipedia.org/wiki/Median_income).  This is not
available through an API, so I just copied the few required values
manually.

Project motivation
------------------

The annual StackOverflow developer surveys collects responses from
programmers all over the world.  Analyses [by one of the nanodegree
instructors](https://github.com/jjrunner/stackoverflow) and by other
colleagues have found that country of residence is one of the
variables most strongly related to salary.  My goal here is to make
some further country-by-country comparisons.  Specifically, I ask the
following questions:

1. How do developer salaries vary across countries, in comparison with
   the general national income levels?
2. Can we observe a significant gender pay gap in the IT sector, and
   does that vary significantly across countries?
3. In which countries are developers the most satisfied with their
   jobs?

Again, see the [report](blog.md) for the results!

License and acknowledgments
---------------------------

I would like to thank StackOverflow for making public their
interesting survey results.  I also acknowledge the use of OECD
econometric data and the Gallup poll on median incomes.

Feel free to use any of the code in this repo if you find it useful ☺.
