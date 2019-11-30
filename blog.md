How do salaries and work conditions in the IT sector vary across
countries?  Evidently, culture and economic reality are vastly
different across countries.  On the other hand, the IT sector is very
globalized.  How do these two facts play against each other?

The goal of this blog post is to gain some insight on this issue.  We
pose the following questions:

1. How do developer salaries vary across countries, in comparison with
   the general national income levels?
2. Can we observe a significant gender pay gap in the IT sector, and
   does that vary significantly across countries?
   
Developer salaries across countries
-----------------------------------

The IT sector is very globalized, both in terms of the tools and
technologies available to developers in different countries, and in
terms of movement of workers.  This might lead us to suspect that
developer salaries in different countries do not vary as drastically
as the general national figures do.  On the other hand, your salary as
a developer depends a lot on *what kind* of development you do [ref to
jake], and the types of jobs available in different countries vary a
lot too; so this might counter the “globalization” effect.

To see how these forces (and others) play out, the figure below shows
the median national income in various countries and the median income
of respondents of the 2018 StackOverflow developer survey, broken down
by country.  We focus on those countries where at least 500 full-time
employed survey respondents reported their salary.

![National median incomes versus respondent's median
income](median-salaries.png)

What we see here is that the median developer income is above the
national median income everywhere, usually substantially so.  This
difference ranges from a 13% increase in Sweden to an 11-fold increase
(!!!) in India.

The figure above dispels any notion that the IT sector is more
egalitarian, in a comparison across countries.  But it is interesting
to note that the median developer salary in many less wealthy
countries is pretty much comparable with the general median income of
rich countries: compare Russia and Brazil with Spain and Italy, or
Poland with Germay, UK and France.

It's also interesting to compare developers salaries across countries
in terms of their purchasing power.  Here, we show the median SO
survey respondent salary adjusted by PPP index.  Under this metric, we
still see large differences across countries, but some interesting
things happen: Poland and Russia now get close, or surpass, the richer
Western European countries.  The median purchase power of a developer
in Brazil and India is comparable to that of the general population
in the developed countries.

![Survey respondent median income, PPP adjusted](median-salaries-ppp.png)

Gender matters
--------------

It's no secret that the software industry has serious gender balance
issues, at least when it comes the amount of female representation in
the field.  This is the percentage of male respondents, among those
who reported a gender:

| ITA  | BRA  | SWE  | ESP  | POL  | DEU  | FRA  | NLD  | RUS  | AUS  | GBR  | IND  | CAN  | USA  |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 96.9 | 95.6 | 95.1 | 94.4 | 94.2 | 94.2 | 94.0 | 93.6 | 93.6 | 92.8 | 92.6 | 92.5 | 89.6 | 89.5 | 

Now, one may ask if, once a female breaks into the field, there will
still be significant differences in their career outcome, compared the
her male peers.  One metric for this is the gender *wage gap*, defined
as follows by the OECD:

> “The gender wage gap is defined as the difference between median
> earnings of men and women relative to median earnings of men. Data
> refer to full-time employees on the one hand and to self-employed on
> the other.”

In other words, this is the percentage penalty, in median income,
received from being female.  The OECD provides this statistic for the
general workforce in several countries, and we computed the
corresponding value among survey respondents, restricting to the case
of full-time employees.

![Wage gender gap by country, in general and among survey
respondents](wage-gap.png)

This result is striking.  First, it dispels any idea that the only
difference between men and woman, in career terms, is numerical.
Moreover, is little general relation between the wage gap in the IT
sector and in the broader workforce across countries.  Netherlands,
Germany and Canada fare comparatively well in pay balance for
developers, although this is not the case for the broader workforce;
and France, Spain and Australia, which have the best wage gap figures
for the broad workforce, do not look good, even in relative terms,
when we focus on the IT sector.


Notes and caveats
-----------------

National median income data is from the OECD and refers to working-age
population (18–65).  For each country, we use the most recent
avaliable figure, which in some cases is ...

