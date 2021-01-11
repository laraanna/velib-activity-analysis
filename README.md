# Velib Activity Analysis 
## before and during the first lockdown in Paris

### 1. Get Started
```bash
git clone git@github.com:laraanna/velib-activity-analysis.git
cd velib-activity-analysis
```
Open the notebook in a data science notebook of your prefence.

### 2. Research Question
- How many Velib bikes can we find in Paris and how are they distributed throughout the city?
- How did the bike usage change during lockdown?
- Which stations gained vs. lost bikes between 8-10am on the first day of lockdown? (compare to same day pre-lockdown)
- How did the bike usage change over the entire period per arrondissement?

### 3. Dataset
Velib is large-scale public bicycle sharing system in Paris, France. The data is openly accessible on the the [Paris City data](https://opendata.paris.fr/explore/?disjunctive.theme&disjunctive.publisher&disjunctive.keyword&disjunctive.modified&disjunctive.features&sort=modified&q=velib) website. 

1. The data was taken from [here](https://pub.phyks.me/datasets/velib/2020/) in the form of SQL. I took the data of week 11 and 12 from 2020. 
    - Week 11 (09/03/2020 - 15/03/2020)
    - Week 12 (16/03/2020 - 22/03/2020)
    

2. In the notebook "Velib - Data Preperation" the data was extracted and converted to be presented in a dataframe


Characteristics on velib station data:
- **station_id:** unique ID of the bike station	
- **name:** name of the bike station
- **latitude:** geographic coordinate (north–south position) 
- **longitude:** geographic coordinate (east–west position) 
- **bike_stands:** available bike stands at this station
- **banking**
- **bonus** 
    
Velib data on disponibility in real time:
- **station_id:** unique ID of the bike station
- **available_bikes:** availble bikes at the station
- **available_ebikes:** availble e-bikes at the station
- **free_stands:** inidcates the number of free stands at the station
- **status:** indicates whether the station is operating or closed
- **updated:** the timestamp of the update

### 4. Preview
#### Timelapse of station activity 11/03/2020 (Wednesday before lockdown)
![wed_prelockdown_timelapse](/assets/wed_prelockdown_timelapse.gif)
#### Timelapse of station activity 18/03/2020 (Wednesday first day of lockdown)
![wed_lockdown_timelapse](/assets/wed_lockdown_timelapse.gif)


