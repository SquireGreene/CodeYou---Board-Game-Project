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
- What are the most populat themes in my playgroup?

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

### Required Features
As per the project guidelines I have incorporated the following 5 features into this project:
1. **Loading Data:** Read TWO data files (JSON, CSV, Excel, etc.). AND Set up a local database and read data in with SQLite or SQLAlchemy
2. **Clean and Operate on Data While Combining Them:** Clean your data and perform a SQL join with your data sets using either plain sql or the pandasql Python library.
3. **Visualize / Present your data:** Make 3 matplotlib or seaborn (or another plotting library) visualizations to display your data.
4. **Best practices:** Utilize a virtual environment and include instructions in your README on how the user should set one up.
5. **Interpretation of your data:** Annotate your code with markdown cells in Jupyter Notebook, write clear code comments, and have a well-written README.md. 

### Insights
Fill in some insights later.


<img src="https://zenandraine.files.wordpress.com/2015/12/game-over-thank-you-for-playing-saying-quotes-pictures.jpg" width="500" height="300">
