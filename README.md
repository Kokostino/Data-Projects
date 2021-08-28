# Personal_Projects

- **Aesthetics.ipynb**:<br />

  **Goal**: Order images by similarity of their dominant colours for aesthetics.<br />
  **Method**: Finding the dominant colours in images using KMeans, calculating distances in Cielab colour space using the metric Cielab ΔE* CIEDE2000 to account for distances as perceived by the human eye. Second KMeans clustering to find clusters of images which look aesthetically together colourwise.<br />
    The left side shows the original image, while the right depicts the dominant colours of the corresponding image clustered with KMeans and RGB. One can see that the dominant colours in the last image are particularly off, since perception of lighting is a major factor for using ciede2000.<br />
  ![alt text](https://github.com/Kokostino/Personal_Projects/blob/master/cluster1.PNG?raw=true)<br />
  **In progress**: Currently, KMeans and RGB coordinates (having a euclidean metric) is used for finding the dominant colours in an image. Ideally one'd use Lab space and ΔE*-metric. In **Aesthetics_KMedoids.ipynb** we use KMediods for clustering which also works for non-euclidean distances.<br />
  The upper image shows dominant colours found via KMedoids, the lower one via KMean. The clustered image is the last one from the previous plot, where the colours by KMeans were a bit off.<br />
  ![alt text](https://github.com/Kokostino/Personal_Projects/blob/master/MedvsMean.PNG?raw=true)<br />
  

- **Animal_Attacks_in_North_America.ipynb**:<br />

  **Goal**: Get some idea about the local distribution of fatal animal attacks in North America.<br />
  **Method**: Scraping data regarding fatal animal attacks from wikipedia, extracting spatial information & transforming to coordinates using geocoder and plotting it with folium:

![alt text](https://github.com/Kokostino/Personal_Projects/blob/master/map_animal_attacks.PNG?raw=true)<br />
  **In progress**: Add serial killer data.<br />
**Issues**: Data from Wikipedia tremendously lacks completeness regarding animal attacks.
