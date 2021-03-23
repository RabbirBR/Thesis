# Update Log
## Things to know
The log will be in the order of newest to oldest.

## 14-01-2020
### Done -
1. Found NOAA Whale information page.
    - [Link to page](https://www.fisheries.noaa.gov/whales)
2. [2017 Aerial Surveys of Arctic Marine Mammals](https://www.fisheries.noaa.gov/resource/data/2017-aerial-surveys-arctic-marine-mammals).
3. Sent a request to the MASATI (MAritime SATellite Imagery) Dataset [Link to page](https://www.iuii.ua.es/datasets/masati/).
4. Airbus Ship detection database [Kaggle link](https://www.kaggle.com/c/airbus-ship-detection/data).
5. NOAA Fisheries Steller Sea Lion Population Count [Kaggle Link](https://www.kaggle.com/c/noaa-fisheries-steller-sea-lion-population-count/rules).
6. [Curated Sentinel 1 & 2 dataset](https://mediatum.ub.tum.de/1474000).
7. [The Science of finding whales](https://www.fisheries.noaa.gov/feature-story/tracking-technology-science-finding-whales).
8. [NASA Funded WhaleWatch Program](https://www.fisheries.noaa.gov/west-coast/marine-mammal-protection/whalewatch).
9. [WhaleTrack](https://en.uit.no/prosjekter/prosjekt?p_document_id=505966).
    - Tracks 900 individual humpback whales.
    - Might be useful for knowing exact locations of whales to find recent and old pictures in the satellite images.
10. Built a CNN that is able to identify whales or not whales with an accuracy of 91.91%.
11. Found a some papers relating to the aerial photos of whales in kaggle -
    - [Dataset link](https://www.kaggle.com/c/noaa-right-whale-recognition/data).
    - "Saving the whales with image processing" [Link to paper](https://web.stanford.edu/class/ee368/Project_Autumn_1516/Reports/Ahres_Kangaspunta.pdf).
    - Right Whale Recognition [Link to paper](http://sumitg.com/assets/right-whale.pdf)

### Challenges -
1. An idea to improve the whale detection in an image using image processing. General Idea:
    - Find objects in the image (Can be made much easier with the infrared images to get objects with heat signatures. E.g. Animals/Ship/AirCrafts).
    - For each object:
        - Take the contour of the object and copy the object pixels from the image to another image.
        - Make the image a square with black or white background and only the object.
        - Convert the square to a common smaller size (say 128-128 or even 32-32).
        - Classify if the object is whale or not.
2. Downsampling and trying on different size images in descending order.
3. Rewriting Proposal for ESA Worldview-3 Satellite.

### Next Steps -
1. Finding more overhead image datasets of oceans or overhead images in general. (Aircraft/Drone/Satellite).
2. Trying to find additional methods and papers.


## 10-01-2020
### Done -
1. Found Sentinel-2 Toolbox 
    - [Toolbox Explanation page](http://step.esa.int/main/toolboxes/sentinel-2-toolbox/).
    - [Sentinels Aplication Platform(SNAP) download link](http://step.esa.int/main/download/snap-download/).
2. Found a dataset of aerial photos of whales in kaggle -
    - [Article link](https://deepsense.ai/deep-learning-right-whale-recognition-kaggle/).
    - [Dataset link](https://www.kaggle.com/c/noaa-right-whale-recognition/data).
    - Original idea of this dataset is to use face recognition for whales to identify individual whales.
    - Found few papers related to this dataset. 
        - "Saving the whales with image processing" [Link to paper](https://web.stanford.edu/class/ee368/Project_Autumn_1516/Reports/Ahres_Kangaspunta.pdf).
        - Right Whale Recognition [Link to paper](http://sumitg.com/assets/right-whale.pdf)
3. Found a dataset of photos of humpback whales in kaggle
    - [Link to dataset](https://www.kaggle.com/c/humpback-whale-identification/data)
    - Contains images of whale tail fins.
4. Alternative way of detecting Whales using deep CNN.
    - Uses CNNs to construct an echolocation click detector designed to classify spectrograms generated from sperm whale acoustic data according to the presence or absence of a click.
    - Deep Machine Learning Techniques for the Detection and Classification of Sperm Whale Bioacoustics.
    - [Link to paper](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6715799/)
    

### Challenges -
1. Trying to use the dataset for training a CNN for whale detection.
    - First with the images as is and then with lower resolution of the same test images.

### Next Steps -
1. Finding satellite datasets.
2. Studying more published papers.


## 07-01-2020
### Done -
- Emailed the authors of [[1]](References.md).
- Created account with ESA to apply for Dataset.
- ESA SPACEWHALE program [Link to page](https://business.esa.int/projects/spacewhale).
    - The SPACEWHALE kick start project was launched in April 2018 and was successfully completed in December 2018. The SPACEWHALE algorithm accurately detected whales in satellite imagery independent of training images, thus proving the concept and technical feasibility. SPACEWHALE was able to achieve 100% accuracy on the identification of large whales in test imagery for this kick-start activity. The program can now be applied to new areas via a follow-up demonstration project.
    - Might be useful information for applying to Worldview-3 dataset.
    - Key Difference - The original paper studied specific species of whales and it was done using feature detection to detect key features of the whales, this program uses a Convolutional Neural Network to detect whales in general.
- Looked up the Sentinel Satellites and Copernicus Program. [Link to Copernicus program Overview](https://www.esa.int/Applications/Observing_the_Earth/Copernicus/Overview4).
    - <b>Sentinel-2</b> and <b>Sentinel-6</b> programs might be relevant to the thesis as they are both focused on oceanography, among other things.
- Looked for open data for images of whales from overhead (Aircraft/Ships/Satellite).
    - [[2]](References.md) Found a dataset collected and organized by NOAA. This tracks mammals around the Ocean near Alaska using aeroplane and ships. A list of known locations may help narrow the search of starting points when we have the image data. [Link to the Dataset](https://catalog.data.gov/dataset/marine-mammal-observations-collected-by-aircraft-and-ship-and-submitted-as-part-of-the-conocoph89110).
- Found a paper studying whale behaviour in different situations using drones. (Ex: While traveling, while they are near other whales, etc.) [Link to paper](https://www.frontiersin.org/articles/10.3389/fmars.2018.00319/full).


### Challenges -
- First author, Hannah C. Cubaynes, in paper [[1]](References.md) is away on vacation until 22nd January. Also mailed co-authors, waiting for reply.
- There are many things in the form for applying for the Worldview-3 dataset. Might be best to apply with guidance of the supervisor.

### Next Steps -
- Studying the datasets found.
- Studying more published papers before meeting in 16th January.