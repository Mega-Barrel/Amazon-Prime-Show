# Amazon-Prime-TV-Show

Data Source: [Amazon Prime TV shows](https://www.kaggle.com/nilimajauhari/amazon-prime-tv-shows)

**Some Brief content**

>The data set contains the name of the show or title, year of the release which is the year in which the show was released or went on-air, No.of seasons means the number of seasons of the show which are available on Prime, Language is for the audio language of the show and does not take into consideration the language of the subtitles, genre of the show like Kids, Drama, Action and so on, IMDB ratings of the show: though for many tv shows and kid shows the rating was not available, Age of Viewers is to specify the age of the target audience- All in age means that the content is not restricted to any particular age group and all audiences can view it.

# Result/Analysis Outcome

- Kids, Action, Drama, Comedy are the most watched Genre.
- Most of the TV Shows are in English language > 400 Series followed by Hindi Language < 50.
- The Year 2018 had Highest Number of TV shows releases > 75, followed by the year 2019, 2017 and 2016
- The TV shows ```[Forensic Files, NCIS, Grey's Anatomy, Supernatural, Doctor Who, Two and a Half Men, The Big Bang Theory, Blue Bloods, Shameless, Hawaii Five-O]``` have Seasons >= 10.

# Download the Project
```
# Clone or Download the Repository

- To clone: $ git clone https://github.com/Mega-Barrel/Amazon-Prime-Show.git

# Install the numpy, pandas, seaborn, matplotlib libraries.
```

# Checking the Null Values

```python
# Check for total Null values present
df.isnull().sum()
```
## ***Output***

Name of the show :            0

Year of release :             0

No of seasons available :     0

Language :                    0

Genre :                       0

IMDb rating :               283

Age of viewers :              0

# ***Using Median To fill the IMDb rating, Null Values***
```python
fill_val = df['IMDb rating'].median()
df['IMDb rating'].fillna(fill_val, inplace=True)
```

# Displaying some Visualization

- Plot for TV Show Genre released in 2020
![Recent_releases](images/recent_release.png)

- Pair Plot for TV shows
![Pair_Plot](images/pair_plot.png)

- Count Plot for TV shows Genre for the Data.
![Count_Plot](images/Count_Plot.png)

- Count Plot for Age Group
![age_viewers](images/Age_viewers.png)

- Pair Plot for Languages used in Shows
![language](images/Language.png)

- Plot for TV shows released in following Years
![year_Plot](images/Year_Count.png)

- Joint Plot
![Joint_Plot](images/Joint_Plot.png)

- Plot for IMDb Rating as per Languages
![line_Plot](images/Line_Plot.png)

- Pair Plot for TV shows
  ![Pair_Plot](images/pair_plot.png)


# ***Enough of Data Visualization 😒🤦‍♂️, Some key findings***

- TV show Popular By Hindi Language
  
![Language](Code_Blocks/Popular_Hindi_language.png)

- TV show Popular By English Language
  
![Language](Code_Blocks/Popular_English_language.png)

- TV show Popular By among Kids
  
![Language](Code_Blocks/Popular_Kids_Shows.png)

- TV show Popular By Drama Genre
  
![Language](Code_Blocks/Drama_Genre.png)

- TV show Popular By Action Genre
  
![Language](Code_Blocks/Action.png)

- TV show Popular By Horror Genre 😱🧛‍♂️
  
![Language](Code_Blocks/Horror.png)
Sad Only 1 Movie In ```Horror``` Genre 😭

- TV show Popular By Drama, Comedy
  
![Language](Code_Blocks/D_C.png)


- Popular TV show for max number of seasons with IMDb > 8 ratings
  
![Language](Code_Blocks/IMDB_rating.png)

# ***Word Clouds***

### **Word Cloud For TV Series**
![TV](images/Shows_Word_Cloud.png)

### **Word Cloud For Genre**
![TV](images/Genre_Word_Cloud.png)