# Are People Still Talking About Buffy?
## Let's look at Spotify podcast data to find out.
Submitted June 25, 2023

Read the project <a href="https://retrospatial.github.io/buffy-podcasts/">here</a>!


### Description
As a Buffy lover and podcast listener, I wanted to investigate the show's cultural legacy by analyzing Spotify podcast data and visualizing certain trends over time, namely: when these podcasts were first published, how long a podcast typically went on for, what cultural phenomena coincided with peaks or troughs in episode numbers (e.g. the show's 20-year anniversary in 2017), and, potentially, what shows/movies/subjects the hosts tended to switch to between Buffy-focused episodes or after they had finished discussing the entire show. <u>This</u> was the story I intended (and still intend!) to pursue, but this first iteration of the project focuses on the number of episodes over time and between different podcasts. 

### Data Collection and Analysis
Some background: I spent most of the week testing out different topics (whether grocery shoppers preferred pulpy vs non-pulpy orange juice, how many times Nebula (the Guardians of the Galaxy character) appeared in Marvel comics before and after the movies, and whether year-based questions in Jeopardy tended to be valued at lower or higher dollar prizes -- which you can find <a href="https://www.datawrapper.de/_/dVC0j/">here</a>). In the end, I used the <a href="https://developer.spotify.com/documentation/web-api/reference/search">Spotify for Developers API</a> to search for podcast shows and episodes containing the keyword "buffy the vampire slayer". I spent some time trying to retrieve the data in different ways as I felt like a lot of information was missing, but ultimately had to work with what I had to create the final visualizations. I used pandas to collect the release date of each episode and grouped the dates by their years, before visualizing them as a line chart on DataWrapper. For the second visualization, I pulled relevant information from the data and created a csv file from it, which I then plugged into Tableau to create the treemap. 

### Findings
Based on the data I managed to pull from the API (which I suspect is not entirely accurate, based on gut instinct and the noticeable absence of my own favorite podcast), I found that the earliest Buffy-related podcast on Spotify was created in 2013 (possibly backdated, as podcasts became available on the app in 2015) and the number of episodes saw a massive rise on the onset of the pandemic in 2020. With the second visualization, I consolidated details about available podcasts on a Tableau treemap and sorted the tiles by the number of podcasts, as I personally like lengthier shows that I can sink my teeth into and wanted to find out what I could listen to next.

### Reflection
Truthfully, I probably would've been able to turn in a more complete project if I had continued down the Jeopardy path, but I really wanted to see this Buffy one through, just out of my love for this show and the people who love it. I definitely wish I had more time and guidance to figure out what went wrong with the API request. Before Spotify, I initially tried to use <a href="https://www.listennotes.com/api/">Listen Notes API</a> and did some work with that data before hitting a paywalled quota, which meant I had to start all over again (plus, they had a beautiful CSV file with all the information I needed -- for $4,200.) Interestingly, I think I grew most in the HTML design side of things, as I wanted the layout (including the color scheme and fonts) to reflect the subject matter, so I took some time to learn how to format the page. 

