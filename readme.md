<img src="http://www.analoggames.com/wp-content/uploads/2016/03/board_game_shelf_shelves_card_analoggames_analog_games_01.jpg" width="500" height="300">

### Why this project?
---
I have been a avid board gamer most of my life, and I find one of the most difficult parts of the hobby is selecting the best game to play with a particular playgroup. I wanted to poll my friends and family about their favorite games and find insights in that data that would better inform me as to which style of games to play with what groups of players. 

I chose to use a BoardGameGeek.com dataset to compare against the list of my playgroup's favorite games. BoardGameGeek.com is considered the IMDB of board gaming and collects lots of data on board games, including crowd sourced ratings and rankings. 

### Datasets
---
I used a combination of two datasets to complete this project. First, I used the Google Form found [here.](https://forms.gle/EBQmShd3iAuLSm35A) to collect the top 5 favorite board games from my friends and family.

This dataset was cleaned a bit, and I added the BoardGameGeek.com IDs for each board game to create the FavoriteGames.csv file in this repository.

Then I also used a dataset from BoardGameGeek itself, that I cound on Kaggle [here.](https://www.kaggle.com/datasets/andrewmvd/board-games)

This raw file can be found in this repository as the bgg_dataset.csv.

I then used the code found in the CreateSQLdb file in thie repository to create a SQLlite database containing these two datasets. This is the boardgame_data.db file.

### My Data Journey
---

My data anlysis is more explicitly addressed in the markdown sections of the DataINvestigation of the Jupiter Notebook, but I will also offer a brief overview here. My goals were to look specifically at the following insights:

- Who in my playgroup likes the highest rated games?
- Who in my playgroup likes the most complex games?
- What are the most popular games in my playgroup?
- Who in my playgroup likes the newest and the oldest games?
- What are the most popular mechanics in my playgroup?
- What are the most popular genres in my playgroup?

The bulk of this project uses a Jupiter Notebook to give insight into these questions and create visualizations to better understand these insights.

### How to Replicate this Analysis
---
To replicate this proect please follow the steps below:
1. Clone the repository to your machine:
    '''bash git clone https://github.com/SquireGreene/CodeYou---Board-Game-Project'''
2. Create and activate a virtual environment, and install required packages from 'requirements.txt':
    - **Linux/Mac:**
      ```bash
      python3 -m venv venv
      source venv/bin/activate
      pip install -r requirements.txt
      deactivate
      ```
    - **GitBash:**
      ```bash
      python -m venv venv
      source venv/Scripts/activate
      pip install -r requirements.txt
      deactivate
3. Open up the DataInvestigation.ipynb and enjoy!

### Required Features
As per the project guidelines I have incorporated the following 5 features into this project:
1. **Loading Data:** Read TWO data files (JSON, CSV, Excel, etc.). AND Set up a local database and read data in with SQLite or SQLAlchemy
2. **Clean and Operate on Data While Combining Them:** Clean your data and perform a SQL join with your data sets using either plain sql or the pandasql Python library.
3. **Visualize / Present your data:** Make 3 matplotlib or seaborn (or another plotting library) visualizations to display your data.
4. **Best practices:** Utilize a virtual environment and include instructions in your README on how the user should set one up.
5. **Interpretation of your data:** Annotate your code with markdown cells in Jupyter Notebook, write clear code comments, and have a well-written README.md. 

### Insights
This project was a lot of fun, as it gave me insight into the people closest to me and the types of board games they prefer to play. I especially was interested in seeing where we overlap in taste as a playgroup in game quality,game complexity, and game mechanics -- as well as just game titles themselves.

I expected some of the results gained through this project:

1. The players that liked the highest rated games are some of the folks most interested in the hobby, and therefore the people exposed to the largest variety of games.
2. The players that enjoyed the games with the highest complexity ratings tended to also follow my expectations, as I have been gaming with some of these folks for years and know they like big, complex games. Also, Adam and Travis are not into heavy games like the rest of teh players in my playgroup and that came through in my analysis.
3. It also did not surprise me that Wingspan is the game we have most in common. It is a beautifully produced mid-weight game that has a lot of crowd appeal.

Some things I didn't expect:

1. I did not expect our favorite mechanic to be *income.* I know our group does have a strong bias towards economic games, but I thought it would get beaten out by a mroe core mechanic like *worker placement* or *card drafting*. It goes to show how common "incoming" can be in board games and how prevelant it is as a secondary or additional mechanic.

2. I was also surprised by how many players in my group like Clue! or one of the Clue variants. I will have to look to add a few Clue-like games to my collection!

### Acknowledgements

I'd like to thank Clay, Matt, and John for being excellent mentors during this course as I start my Python and SQL journey! Double shout out to John for helping me with the SQLlite pivot tables. I'd like to thank Rob, Rui, and Ailene for being great classmates, and helping me test my project on their machines. I'd be remiss if I also didn't mention my lovely fiancee Shelley, who continues to support all of my coding endeavors and lets me obsessively pound away on the keyboard some nights!




<img src="https://zenandraine.files.wordpress.com/2015/12/game-over-thank-you-for-playing-saying-quotes-pictures.jpg" width="500" height="300">
