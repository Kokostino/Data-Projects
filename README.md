# Personal_Projects

- **Aesthetics.ipynb**:<br />
  **Goal**: Order images by similarity of their dominant colours for aesthetics.<br />
  **Method**: Finding the dominant colours in images using KMeans, calculating distances in Cielab colour space using the metric Cielab ΔE* CIEDE2000 to account for distances as perceived by the   human eye.<br />
  **In progress**: Automatically finding the nearest neighbours and save to output folder.<br />
  **Issues**: KMeans uses RGB colour space and euclidean metric, while ideally it'd use Lab space and ΔE*-metric. <br />
  Is Cost(making KMeans ΔE*-dependent or transforming input data accordingly to use Euclidean metrics)>>Loss(accuracy)?<br />
  Example:<br />
  The left side shows the original image, while the right depicts the dominant colours of the corresponding image clustered with KMeans and RGB.<br />
  ![alt text](https://github.com/Kokostino/Personal_Projects/blob/master/cluster1.PNG?raw=true)<br />

- **Animal_Attacks_in_North_America.ipynb**:<br />
  **Goal**: Get some idea about the local distribution of fatal animal attacks in North America.<br />
  **Method**: Scraping data regarding fatal animal attacks from wikipedia, extracting spatial information & transforming to coordinates using geocoder and plotting it with folium:

![alt text](https://github.com/Kokostino/Personal_Projects/blob/master/map_animal_attacks.PNG?raw=true)<br />
  **In progress**: Add serial killer data.<br />
**Issues**: Data from Wikipedia tremendously lacks completeness regarding animal attacks.
