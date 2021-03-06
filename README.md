# Steam Level Calculator
:video_game: Steam is a cloud-based gaming library. One of its most popular features is the ability for users to customize there profiles . Every Steam user has a level, with higher levels granting bonuses like extra slots on your friends list and higher drop rates for booster card packs. This web application can help the user to know how much is the cost/badges to get to his wanted level.

### *Features*
- Takes user input (steam username - wanted level) and calculate the cost of rank up
- Calls the steam api from the backend to avoid the CROS error
- Theme selection (dark/light mode)  'will be added soon'

Steam max level cap is 5099 now so anything above that would not get calculated .


### *Demo*

* Source Control: GitHub
* Hosting: This application is deployed on Heroku. Please check it out [Here](https://steamlevelcalculator.herokuapp.com/)

If you want to clone the project make sure to change the Steam_API_Key on the index.js and i recommend using dotenv before deploying your project so you dont share your api key publicly.

![demo](https://raw.githubusercontent.com/Mistydz/SteamLevels/master/public/Demo.png)



### *Technologies & Tools*
##### *Front End*
> Html/CSS/Javascript
##### *Back End*
>Node/Express
##### *API's Used*
>Steam API [Documentation](https://partner.steamgames.com/doc/webapi/IPlayerService)

>REST Countries API [Documentation](https://restcountries.eu/)

### *Releases*
Problem to fix : website is not runing on mozilla firefox (window refresh stop doesnt work) 
#### Version 1.1

- Features
  - Mobile optimisted layout
  - Added user country and flag 
- Fixes
  - Max allowed wanted level as 5099
  - if level wanted is inferior to current level stop calculating 

#### Version 1.0

- Features
  - Steam user data from the steam api (Name,Level,XP)
  - Calcuate the difference on xp betwen current and wanted xp
  - Deployment on https://steamlevelcalculator.herokuapp.com/
