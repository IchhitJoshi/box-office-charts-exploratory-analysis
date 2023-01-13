# Observing and exploring the trends in box office (movie theater) revenues and attributes of yearly top 100 highest grossing movies from 1995 to 2022 (present)

## Introduction to the Data Set:
### The Numbers Box Office Data

The Numbers is a film industry data website that tracks box office revenue in a systematic, algorithmic way. The company also conducts research services and forecasts incomes of film projects. Their website has tabular movie report data for all the top 100 highest grossing movies of every year starting from 1995 to 2022 (present). <br>

This project is only about the box office performance of movies in theaters and doesn’t include any streaming / home-DVD revenues. <br>

I will be fetching yearly data from the years 1995 to 2022, which will equal 28 tables of 100 rows each (data sets), which can be combined into one huge dataset with 2800 rows. <br>

Database Source: <br>
https://www.the-numbers.com  <br>

© 1997-2022 Nash Information Services, LLC. <br>

Every top 100 highest grossing movies data can be generated using their website: <br>
https://www.the-numbers.com/movies/report-builder <br>

One has the option to choose what columns to retrieve for the tables. So, I've chosen some columns that I'll be using in the project.

## Central Questions:
How have the box office revenues of movies changed over the years from 1995 to 2022? What is the most profitable genre of movie to produce? What are the top 10 most expensive movies ever made from 1995 to 2022? What are the top 10 all-time highest grossing movies and what were their profits? Which theater distributor has made the most profit over the years? 

Finally, one last question I would like to answer is: <br>For every distributor, which movie hit the maximum profit out of all their distributed movies? What year did it happen and how much was the profit?

### Why is this data and problem interesting?

Movie theaters have always been the major source of entertainment for millions of people across the globe and it's also the core source of income for the production companies that produce the movies. Production companies, being profit-oriented, will always try to maximize the profits they can earn from the box office. <br>

Now, with the rise of streaming services, it is interesting to see if there has been any decline of box office revenues in recent years. Are people still going to the theaters to watch movies? Such question can be answered if we had all the revenue data over the years. This is one of the major goals of this project. <br>

The Numbers website, which is the data source for this project, has all the production budget allocated by the production companies and the box office revenue earned domestically and globally for the top 100 highest grossing movies from 1995 to 2022. <br>

One of the interesting questions that I'm looking forward to answering through this project is knowing what are the top 10 movies all-time that have made the most amount of profit.  <br>

This data has a lot of potential. Are superhero and fictional movies making the most profit in the box office? Looking at the correlation between genre and profit can be helpful for production companies. If there is any significant proof that a specific genre can make the most money, this would help companies to focus on what type of content to create for the audience. <br>

We can also see if any specific distribution/production companies like Universal Studios or Walt Disney have dominated the box office charts over the years.  <br>

Overall, I think this data can be really useful for the production companies to help make decisions on maximizing their profits. <br>

### Dataset Description:

I will be fetching yearly data from the years 1995 to 2022, which will equal 27 tables of 100 rows each (data sets), which can be combined into one huge dataset with 2700 rows.

Every yearly table from the source website will contain the following columns:
 
Rank:
Data Type: int

Rank of the movie ranging from 1 to 100 based on highest revenue to lowest revenue

Release Year:
Data Type: int

Ranges from 1995 to 2022
It is the year the movie was released in the domestic market.

Release Date:
Data Type: string

Ranges from “January 1, 1995” to “December 31, 2022”
It is the date when the movie was released in the domestic market.

Movie Title:
Data Type: string

Official name of the movie released in the theaters

Theatrical Distributor:
Data Type: string

Company responsible for the marketing of a film. The distribution company may be the same with, or different from, the production company. For example, Sony Pictures is a Theatrical Distributor.

Genre:
Data Type: string (categorical)

Stylistic categories where a particular movie can be placed based on the setting, characters, plot, mood, tone, and theme.

Can be one of the following:

Adventure
Action
Drama
Comedy
Thriller/Suspense
Horror
Romantic Comedy
Musical
Documentary
Black Comedy
Western
Concert/Performance
Multiple Genres
Reality
Educational

Source:
Data Type: string (categorical)

Source from which the plot of the movie is based on.

Can be one of the following:

Original Screenplay
Based on Fiction Book/Short Story
Based on Comic/Graphic Novel
Remake
Based on Real Life Events
Based on TV
Based on Factual Book/Article
Spin-Off
Based on Folk Tale/Legend/Fairytale
Based on Game
Based on Play	
Based on Theme Park Ride
Based on Toy
Based on Religious Text
Based on Short Film
Based on Musical or Opera
Based on Movie
Compilation
Based on Song
Based on Musical Group
Based on Web Series	
Based on Ballet
Based on Radio

Production Method:
Data Type: string (categorical)

The method by which the movie is made. For example, if using humans as actors, then the production method is live action.

Can be one of the following:

Live Action
Animation/Live Action
Digital Animation
Hand Animation
Stop-Motion Animation
Multiple Production Methods
Rotoscoping


Creative Type:
Data Type: string (categorical)

Categories where a movie can be placed. (similar to genre but descriptive in a different way)

Can be one of the following:

Contemporary Fiction
Kids Fiction
Science Fiction
Super Hero
Fantasy
Historical Fiction
Dramatization
Factual
Multiple Creative Types

Production Budget:
Data Type: int

The amount of money it cost to make the movie including pre-production, film and post-production, but excluding distribution costs.

Domestic Box Office: 
Data Type: int

Total money spent on tickets by moviegoers in the “domestic market”, which is defined as the United States, Canada, Puerto Rico and Guam.

Inflation Adjusted Domestic Box Office:
Data Type: int

The domestic box office revenue but adjusted to the current inflation rate. So, the revenue a movie released in 1995 would’ve actually earned if it was released today.

International Box Office: 
Data Type: int

Total money spent on tickets by moviegoers in the “international market”, which is defined as everywhere outside the United States, Canada, Puerto Rico and Guam.

Worldwide Box Office: 
Data Type: int

Sum of Domestic Box Office and International Box Office


