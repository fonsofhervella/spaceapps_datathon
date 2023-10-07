![Copy of MDA II Final Presentation (2)](https://www.eoportal.org/ftp/satellite-missions/d/DSCOVR_081221/DSCOVR_Auto23.jpeg)




&nbsp;

<!-- About the Project -->
# :star2: DSCOVER Oracle Project

The Deep Space Climate Observatory (DSCOVR), can measure the strength and speed of the solar wind in space, which enables us to predict geomagnetic storms that can severely impact important systems like GPS and electrical power grids on Earth. It acts like a sensor buoy at sea that warns of an oncoming tsunami—DSCOVR can warn forecasters 15 to 60 minutes before a storm of particles and magnetic field, known as a coronal mass ejection (or CME) reaches earth. However, it continues to operate past its expected lifetime and produces occasional faults that may themselves be indicators of space weather (the launch was in Feb. 11 2015, the arrival l at Sun–Earth L1 Lagrange point in Jun 8, 2015, and was expected to last 5 years)

DSCOVR orbits about a million miles from Earth in a unique location called Lagrange point 1, which basically allows it to hover between the Sun and our planet. From that vantage point, DSCOVR measures the plasma that may cause geomagnetic storms hours before it reaches us– ideally providing an early warning of what’s coming our way. The time that it takes for that plasma to reach Earth and trigger a geomagnetic storm might be anywhere from about 15 minutes to a few hours. 

DSCOVR uses 2 main space weather instruments 

    Magnetometer: Measures solar wind magnetic field vector. Given dataset has 3 features: x, y and z.

    Faraday Cup: Provides real-time measurement of solar wind proton density, speed, velocity, temperature, etc... NASA and NOAA (SWPC and OSPO) are actively monitoring Faraday Cup behavior in various solar wind conditions, and developing or updating flight software solutions to optimize the instrument behavior. The most recent modification was performed in August 2020, and additional work is ongoing. Given dataset has 50 features.

![MDA II Final Presentation](https://www.nesdis.noaa.gov/s3/migrated/point_of_lagrange1_big_0.jpg)

DSCOVR uses measurements of the solar wind density, temperature, speed, and magnetic field to run computer simulations of the Earth's magnetic field and atmosphere. Based on those simulations, NOAA forecasts when a geomagnetic storm will occur and how strong it will be. The strength of the geomagnetic storm is measured on a scale called the Planetary K-index (Kp). 

The instrument onboard DSCOVR that measures the solar wind's magnetic field continues to function very well, the instrument that measures the solar wind density, temperature, and speed has lost sensitivity and experiences faults and anomalies from time to time. 

### CHALLENGE: 

As a part of the NASA Space Apps Challenge, the project must predict the risk of geomagnetic storms on a 3 hour basis on Earth following the K-Index Scale

The K-index is a scale ranging from 0 to 9, with higher values indicating more severe geomagnetic disturbances. Here's what the different K-index values represent:

    Kp = 0: Very quiet geomagnetic conditions.
    Kp = 1: Quiet geomagnetic conditions with minimal disturbance.
    Kp = 2: Slightly disturbed geomagnetic conditions.
    Kp = 3: Unsettled geomagnetic conditions.
    Kp = 4: Active geomagnetic conditions.
    Kp = 5: Minor geomagnetic storm.
    Kp = 6: Major geomagnetic storm.
    Kp = 7: Severe geomagnetic storm.
    Kp = 8: Very severe geomagnetic storm.
    Kp = 9: Extremely severe geomagnetic storm.

<!-- TechStack -->
# :space_invader: Python Libraries

Here's a brief high-level overview of the tech stack the project uses:

- Pandas: For Data Wrangling to merge data [PANDAS] https://pandas.pydata.org/





<!-- Features -->
# :dart: Algorithms

- By ingesting data from the [Spotify API](https://developer.spotify.com/documentation/web-api/) we combine and rank a selection of artists by analyzing top charts, frequency of appearance, followers and popularity and generate reccommendations relevant to tour managers, festival organizers to support their decision making.


# :bookmark_tabs: Documentation

You can find our documentation [here](https://github.com/Callisthenes/music_industry_intelligence/documentation) with the following tutorials

- **Update Nifi:** Updates done in the course environment that allowed us to stream ingest from Twitter leveraging NIFI processor. 
- **Spotify Config Ingestion:** Step by step guidance of Spotify ingestion leveraging Postman and NIFI.
- **Tweepy tutorial:** Step by step guidance on how to ingest from twitter leveraging Tweepy and NIFI.
- **Two objects working with VM environment:** Sharing a workaround to be able to work with 2 os.environment on the same Jupyter notebook which allowed us to work both with Graphframes and Mariadb.
- **Connect Powerbi to VM environment:** Step by step guidance on how to connect the course environment to PowerBI and leverage the full potential of analytics

# ✨ Contributors 

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/fonsofhervella"><img src="https://avatars.githubusercontent.com/u/108975841?v=4" width="100px;" alt="Alfonso Hervella"/><br /><sub><b>Alfonso Hervella</b></sub></a><br /><a href="https://github.com/codesandbox/codesandbox-client/commits?author=NinoMaj" title="Documentation">💻</a></td>
    <td align="center"><a href="https://github.com/jni"><img src="https://avatars.githubusercontent.com/u/67459756?v=4" width="100px;" alt="Javier Nieves"/><br /><sub><b>Javier Nieves</b></sub></a><br /><a href="https://github.com/codesandbox/codesandbox-client/commits?author=saurabhdaware" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/Callisthenes"><img src="https://avatars.githubusercontent.com/u/91435423?v=4" width="100px;" alt="Pedro V. Esteban"/><br /><sub><b>Pedro V. Esteban</b></sub></a><br /><a href="https://github.com/codesandbox/codesandbox-client/issues?q=author%3Aaditya211935" title="Bug reports">💻</a></td> 
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

