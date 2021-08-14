# Personal_Projects

- **Aesthetics.ipynb**:<br />
  **Goal**: Order images by similarity of their dominant colours for aesthetics.<br />
  **Method**: Finding the dominant colours in images using KMeans, calculating distances in Cielab colour space using the metric Cielab ΔE* CIEDE2000 to account for distances as perceived by the   human eye.

- **Animal_Attacks_in_North_America.ipynb**:<br />
  **Goal**: Get some idea about the local distribution of fatal animal attacks in North America.<br />
  **Method**: Scraping data regarding fatal animal attacks from wikipedia, extracting spatial information & transforming to coordinates using geocoder and plotting it with folium:

![alt text](https://github.com/Kokostino/Personal_Projects/blob/master/map_animal_attacks.PNG?raw=true)
