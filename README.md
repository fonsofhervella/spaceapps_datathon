![Group Logo](https://github.com/fonsofhervella/spaceapps_datathon/blob/main/graphic_design/header_readme.jpeg) 

&nbsp;

<!-- About the Project -->
# :sunny: :satellite: :earth_americas: DSCOVER Oracle Project :sunny: :satellite: :earth_americas:

The Deep Space Climate Observatory [(DSCOVR)](https://epic.gsfc.nasa.gov), can __measure the strength and speed__ of the solar wind in space, which enables us to predict geomagnetic storms that can severely impact important systems like GPS and electrical power grids on Earth. It acts like a sensor buoy at sea that warns of an oncoming tsunami.

DSCOVR can warn forecasters __15 to 60 minutes__ before a storm of particles and magnetic field, known as a coronal mass ejection (or CME) reaches earth. However, it continues to operate past its expected lifetime and produces occasional faults that may themselves be indicators of space weather (the launch was in Feb. 11 2015, the arrival l at Sun–Earth L1 Lagrange point in Jun 8, 2015, and was expected to last 5 years). The instrument onboard DSCOVR that measures the solar wind's magnetic field continues to function very well, the instrument that measures the solar wind density, temperature, and speed has lost sensitivity and experiences faults and anomalies from time to time. 

![Copy of MDA II Final Presentation (2)](https://www.eoportal.org/ftp/satellite-missions/d/DSCOVR_081221/DSCOVR_Auto23.jpeg)


DSCOVR orbits about a million miles from Earth in a unique location called __Lagrange point 1__ (L1), which allows it to hover between the Sun :sunny: and our planet :earth_americas:. From that vantage point, DSCOVR measures the plasma that may cause geomagnetic storms hours before it reaches us– ideally providing an early warning of what’s coming our way. The time that it takes for that plasma to reach Earth and trigger a geomagnetic storm might be anywhere from about 15 minutes to a few hours. 

![MDA II Final Presentation](https://www.nesdis.noaa.gov/s3/migrated/point_of_lagrange1_big_0.jpg)


DSCOVR uses 2 main space weather instruments:
- Magnetometer: Measures solar wind magnetic field vector. Given dataset has 3 features: x, y and z.
- Faraday Cup: Provides real-time measurement of solar wind proton density, speed, velocity, temperature, etc... NASA and NOAA (SWPC and OSPO) are actively monitoring Faraday Cup behavior in various solar wind conditions, and developing or updating flight software solutions to optimize the instrument behavior. The most recent modification was performed in August 2020, and additional work is ongoing. Given dataset has 50 features.

![MDA II Final Presentation](https://upload.wikimedia.org/wikipedia/commons/a/a4/Deep_Space_Climate_Observatory_spacecraft_diagram.jpg)

DSCOVR uses measurements of the solar wind density, temperature, speed, and magnetic field to run computer simulations of the Earth's magnetic field and atmosphere. Based on those simulations, NOAA forecasts when a geomagnetic storm will occur and how strong it will be. The strength of the geomagnetic storm is measured on a scale called the Planetary K-index (Kp). The K-index is a scale ranging from 0 to 9, with higher values indicating more severe geomagnetic disturbances. Here's what the different K-index values represent:

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


# :rocket: Challenge :rocket: 

As a part of the [NASA Space Apps Challenge](https://www.spaceappschallenge.org/2023/find-a-team/solar-storm-sentinels-of-pidro/), the project must predict the risk of geomagnetic storms on a 3 hour basis on Earth following the K-Index Scale. This project uses Machine and Deep Learning techniques to develop models that can improve the actual predictions given by NOAA (National Oceanic and Atmospheric Administration)

# 💻 Work performed 💻

- EDA: This exercise has been iterative with and executed simultaneously with the Data Cleaning and Feature Engineering ones, allowing to identify potential improvements that have been implemented in the later stages, and so on.
The EDA starts some statistics to later on, display several visualizations with the aim of detecting patterns and correlation between Kp and Ap and the vectors measures of PlasMAG and the different FC measurements.
Found in notebook: [1_Initial_EDA_DSCOVR_data.ipynb](https://github.com/fonsofhervella/spaceapps_datathon/blob/main/1_Initial_EDA_DSCOVR_data.ipynb)
- Data Wrangling: Considering time constraints and the current intervals of Kp, team has decided to aggregate the data transforming it from minutes to 3 hour interval.
Several statistical features covering the measurements that have taken place inside this 3-hours have been created.
Many of the rows are NaN but they are registered as 0. They could be an anomaly, and they can also be indicator of space weather changes, so the approach of discarding the rows, or filling the NaN with other statistical measurements has been rejected by the group. Instead, we have transformed this null existance in a categorical feature, creating new features for each of our variables as ‘Proportion of NaN values’.
The period where DSCOVR was shut down  (from 27 june 2019 to 2 march 2020) has been discarded.
More information could be found in notebook: [2_Cleaning_and_engineering_DSCOVR.ipynb](https://github.com/fonsofhervella/spaceapps_datathon/blob/main/2_Cleaning_and_engineering_DSCOVR.ipynb)



<!-- TechStack -->
# 🐍📚  Python Libraries

Here's a brief high-level overview of the tech stack the project uses:

- [Pandas](https://pandas.pydata.org/): For Data Wrangling to merge data 





<!-- Features -->
# :dart: Algorithms

- By ingesting data from the [Spotify API](https://developer.spotify.com/documentation/web-api/) we combine and rank a selection of artists by analyzing top charts, frequency of appearance, followers and popularity and generate reccommendations relevant to tour managers, festival organizers to support their decision making.


# 🚧 Limitations

Due to time constraints, really complex models, or accurate finetuning, has been difficult to reach. Also, the final aim is to improve also the front page and stablish and alert system for the stakeholders affected. 
The team has directed its efforts into preparing the machine learning pipeline and working on the models, as the predictions made are considered more important for this challenge than the way in which they are displayed.


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

