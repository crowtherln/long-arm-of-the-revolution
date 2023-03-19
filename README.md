# Long Arm of the Revolution? Allegedly Iran-sponsored Attempts to Kill Expatriates, 1979–2012

## Background

As a college student, I assisted Brian Champion with research on allegedly Iran-sponsored attempts to kill Iranian expatriates, as part of a larger project on allegedly state-sponsored extraterritorial attempted killings. We first published our findings on Iran in 2013, making occasional updates through 2017:

> Champion, Brian and Crowther, Lee. "Appendix 1: Selected, allegedly Iran-sponsored attempts to kill Iranian expatriates, 1979–2012" (2013). *Faculty Publications*. 1570. [https://scholarsarchive.byu.edu/facpub/1570](https://scholarsarchive.byu.edu/facpub/1570)

The data in our publication was semi-structured. In 2022, I started looking into making it more structured, which is what led to this repository.

## About Dataset

The dataset documents attempted killings that meet the following criteria:

1. The attempt was made against one or more Iranians.
2. The attempt took place outside of Iran.
3. Some allegation was made that the state of Iran was at least partially responsible for the attempt.

Brian and I were far from the first to document this pattern, but we attempted to fill a gap in the literature by combining breadth, detail, and a thorough citation of sources consulted.

Our survey began with the 1979 assassination of Shahriar Shafigh in Paris and continued up to the 2012 killing of Gelareh Bagherzadeh in Houston. While we tried to be thorough, our survey was not exhaustive.

## Contents

This repository hosts 4 tables that present a simplified version of the data in our publication:

* [Events.csv](https://github.com/crowtherln/long-arm-of-the-revolution/blob/main/dataset/Events.csv) includes time and location data for 86 attempted killings.
* [Targets_Casualties.csv](https://github.com/crowtherln/long-arm-of-the-revolution/blob/main/dataset/Targets_Casualties.csv) includes details for 232–282 people who were targeted, wounded, or killed in the 86 attempts.
* [Sources.csv](https://github.com/crowtherln/long-arm-of-the-revolution/blob/main/dataset/Sources.csv) lists 259 sources that we used to compile the data.
* [Event_Sources.csv](https://github.com/crowtherln/long-arm-of-the-revolution/blob/main/dataset/Event_Sources.csv) indicates which sources document which events and indicates the quality of the sources for that event. It includes 797 event–source pairs.

It also includes an [entity–relationship diagram](https://github.com/crowtherln/long-arm-of-the-revolution/blob/main/schema/long-arm-of-the-revolution_er-diagram.png) and a [relational schema](https://github.com/crowtherln/long-arm-of-the-revolution/blob/main/schema/long-arm-of-the-revolution_relational-schema.png) to show the relationships between the tables.

Otherwise, I am using this repository primarily as a directory to content hosted elsewhere, rather than as a typical repository.

* The above tables are also hosted on [Kaggle](https://www.kaggle.com/datasets/crowtherln/long-arm-of-the-revolution), with some added field descriptions.
* Tableau Public hosts several visualizations of the data:
  * [This visualization](https://public.tableau.com/views/LongArmoftheRevolutionMinimumDeathTollandDocumentationRating/Sheet1?:language=en-US&:display_count=n&:origin=viz_share_link) provides details about each event, focusing on death tolls and documentation quality.
  * [This visualization](https://public.tableau.com/views/LongArmoftheRevolutionTotalEventsbyCountry/Events?:language=en-US&:display_count=n&:origin=viz_share_link) looks at the number of events by country.
  * [This visualization](https://public.tableau.com/views/LongArmoftheRevolutionTotalEventsbyCountryandYear/EventsbyYear?:language=en-US&:display_count=n&:origin=viz_share_link) does the same, but parses the numbers by year.
  * [This visualization](https://public.tableau.com/views/LongArmoftheRevolutionDeathTollbyCountry/DeathToll?:language=en-US&:display_count=n&:origin=viz_share_link) looks at the death toll by country.
  * [This visualization](https://public.tableau.com/views/LongArmoftheRevolutionDeathTollbyCountryandYear/DeathTollbyYear?:language=en-US&:display_count=n&:origin=viz_share_link) does the same, but parses the numbers by year.

## Project Methodology and Limitations

In the early stages of this project, we relied heavily on such sources as Pahlavi (n.d.) and the Foundation for Democracy in Iran (1996). Rather than focus on one specific event, such sources allege and seek to document a pattern of Iran-sponsored attempted killings outside Iran since the Islamic Revolution. We came to refer to such sources as *chronologies*. Many chronologies consider scores, sometimes hundreds, of events taking place across several continents over the course of over fifteen years. Naturally, given the interest required to attempt a compilation of such breadth, most of the chronologies we looked at involved potential conflicts of interest. Consequently, we took their allegations as a skeleton from which to begin, but then sought to corroborate or correct their claims with more reliable sources.

Given the nature of the events that fall under our scope, we judged news articles to be an accessible and reasonably reliable kind of source with which to establish the details surrounding these events. Because most of the targets in our survey were not especially prominent outside their own circles, most of the events we document are not widely discussed in academic literature. Court records are often more reliable than news articles to establish who perpetrated a crime, but they also tend to be less accessible. We thus rely heavily on news articles. Even among news articles, however, our sources are disproportionately taken from English language newspapers for which we had access to archives.

### A Note on Sources

As indicated above, some of our sources are of questionable reliability. We document events for which some *allegation* was made that the state of Iran was at least partially responsible for the attempt. It is not the case that Iranian responsibility has been reliably established for every event we document. Some of our sources had strong incentives to oppose those in power in Iran—for example, we cite Iranians disempowered by the Islamic Revolution, Iranian opposition groups and figures, political extremists, and research funded by states hostile to Iran. While we tried to corroborate their claims with more reliable sources, in many cases we failed to do so. To address this, we attempted to indicate source reliability by grouping sources into 3 classes, with A being more reliable and C being less reliable.

* Class A sources are often published by established news organizations or in academic journals, and typically center on the event in question.
* Class B sources are often published by established news organizations, but typically only allude to the event in question.
* Class C sources often involve potential conflicts of interest and include polemics, opinion pieces, and chronologies.

Some sources fall under one heading for one event but another heading for another event. For example, Hakakian (2011) includes a chronology in the end matter of her book, but rigorously documents the details of the event that is the subject of her book. When our information is from her chronology, we cite her as a "C" source, but when our information is from her account of event 1.1992-08, we cite her as an "A" source. Eder (1980) likewise fits under multiple headings: In an article about 1.1980-01, he mentions 1.1979-01, so we cite him as an "A" source for the former but as a "B" source for the latter.

Even though we attempted to indicate source reliability, our inclusion of an event still implies only the *allegation* of Iranian responsibility. For some events, Iranian responsibility is well-document—for example, for events including but not limited to 1,.1980-02, 1.1988-01, 1.1989-01, 1.1990-03, 1.1991-04, and 1.1992-08, it seems almost indefensible to assert that Iran had nothing to do with the attempt. For others, however, claims of Iranian responsibility may be more spurious. Readers are invited to consult the sources and conduct further research to determine whether an allegation is well-founded.
