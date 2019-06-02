# McMurray-Wabiskaw-preprocessed-datasets
McMurray/Wabiskaw preprocessed datasets + code for getting packaged

Purpose
-------
This repository serves as a place to put datasets preprocessed for specific purposes that originally came from Athabasca Oil Sands Data McMurray/Wabiskaw Oil Sands Deposit - Electronic Data zip file. The original dataset is described in <a href="https://ags.aer.ca/publications/OFR_1994_14.html">Open File Report 1994-14</a> and can be downloaded from <a href="https://ags.aer.ca/publications/SPE_006.html">this webpage</a>.

A first use-case is a place to put McMurray datasets preprocessed to only have data useful for top prediction and facies prediction that are called in Rockhound, a Python package for quickly and easily calling easy to work with geologic datasets into either a pandas array or xarray. This reduces the need to find, clean, and arrange data when all you need is a starter dataset. 


Information About The Original Datasets
-------
The original dataset is a collection of over 2000 wells made public by the Alberta Geological Survey's Alberta Energy Regulator. To quote their webpage, "In 1986, Alberta Geological Survey began a project to map the McMurray Formation and the overlying Wabiskaw Member of the Clearwater Formation in the Athabasca Oil Sands Area. The data that accompany this report are one of the most significant products of the project and will hopefully facilitate future development of the oil sands." It includes well log curves as LAS files and tops in txt files and xls files. There is a word doc and a text file that describes the files and associated metadata. 

_Wynne, D.A., Attalla, M., Berezniuk, T., Brulotte, M., Cotterill, D.K., Strobl, R. and Wightman, D. (1995): Athabasca Oil Sands data McMurray/Wabiskaw oil sands deposit - electronic data; Alberta Research Council, ARC/AGS Special Report 6._

Please go to the links below for more information and the dataset:

Report for Athabasca Oil Sands Data McMurray/Wabiskaw Oil Sands Deposit http://ags.aer.ca/document/OFR/OFR_1994_14.PDF

Electronic data for Athabasca Oil Sands Data McMurray/Wabiskaw Oil Sands Deposit http://ags.aer.ca/publications/SPE_006.html Data is also in the repo folder: SPE_006_originalData of the original repo for this project <a href="https://github.com/JustinGOSSES/MannvilleGroup_Strat_Hackathon/tree/master/SPE_006_originalData">here.</a>

_The Latitude and longitude of the wells is not in the original dataset._ <a href="https://github.com/dalide">@dalide<a> used the Alberta Geological Society's UWI conversion tool to find lat/longs for each of the well UWIs. A CSV with the coordinates of each well's location can be found <a href="https://github.com/JustinGOSSES/MannvilleGroup_Strat_Hackathon/blob/master/well_lat_lng.csv">here.</a> These were then used to find each well's nearest neighbors.

Please note that there are a few misformed .LAS files in the full dataset, so the code in this repository skips those.

If for some reason the well data is not found at the links above, you should be able to find it <a href="https://github.com/JustinGOSSES/MannvilleGroup_Strat_Hackathon/tree/master/SPE_006_originalData">here.</a>

## Credits to Original Dataset Authors:
```
Wynne, D.A., Attalla, M., Berezniuk, T., Berhane, H., Brulotte, M., Cotterill, D.K., Strobl, R.S. and Wightman, D.M. (1994): Athabasca Oil Sands database; McMurray/Wabiskaw deposit; Alberta Research Council, ARC/AGS Open File Report 1994-14, 51 p.
```
Also please see the SPE_006.txt file in the dataset zip file for additional information on contacting the originally authors.

## License and use constraints
In the metadata file for the original datasets <a href="https://github.com/JustinGOSSES/MannvilleGroup_Strat_Hackathon/blob/master/SPE_006_originalData/Metadata/SPE_006.txt">SPE_006.txt</a> the dataset is described as `Access Constraints: Public` and `Use Constraints: Credit to originator/source required. Commercial reproduction not allowed.`

The preprocessed datasets built on the original datasets therefore follow a similar scheme. The license that best matches the use constraints of the original dataset is the <a href="https://creativecommons.org/licenses/by-nc/2.0/legalcode">Attribution-NonCommercial 2.0 Generic (CC BY-NC 2.0)</a> license. A human-readable version of this license is <a href="https://creativecommons.org/licenses/by-nc/2.0/">here</a>. The key points are free to share, must attribute, and non-commercial so please don't try to resell the data.

## Preprocessed datasets derived from original

### Original datasets but with LAS well log files that don't load well separated and geographic coordinates CSV added saved in Zip file
- Location in repository: 
- What is included:
- How to load:

### Preprocessed dataframe for prediction of Top McMurray Pick Saved in single .h5 
- Location in repository: 
- What is included:
- How to load:

### Preprocessed dataframe from facies prediction in single .h5
- Location in repository: 
- What is included:
- How to load:



