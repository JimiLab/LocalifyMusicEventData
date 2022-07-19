# LocalifyMusicEventData

This is the official project repo for the paper [Towards Quantifying the Strength of Music Scenes using Live Event Data](https://drive.google.com/file/d/18UTmw81ZC8x4O-ZRC5MFIMVO32Dk0CAV/view?usp=sharing). The paper has been accepted by the International Society for Music Information Retrieval (ISMIR) Conference 2022. 

## About Our Data

The ```LocalifyMusicEvents-USA-2019``` dataset used in our paper contains information for 308,051 music events that took place in 2019 and from 1,139 US cities, all of which have a population of 10K or more. This dataset consists of data for 28 socioeceonomic indicators, ranging from 6 different categories: Transportation, Population, Economics, Age, Education, and Race. We also introduce the _Live Event Music Rate (LMER)_, a one-dimensional heuristic for measuring the liveness of a music scene, in this dataset. LMER is calculated as the total number of events during 2019 listed in the city divided by the city population according to 2019 Census population estimates. To use this dataset, download it [here](https://github.com/JimiLab/LocalifyMusicEventData/blob/main/LocalifyMusicEvents-USA-2019/data/LocalifyMusicEvents-USA-2019_paper.csv).

We explore the statistical correlations between LMER and the 28 socioeconomic indicators in [this notebook](https://github.com/JimiLab/LocalifyMusicEventData/blob/main/LocalifyMusicEvents-USA-2019/LocalifyMusicEvents-USA-2019_Step1_StatistcalAnalysis.ipynb). 

We grouped the 1,139 cities by population: 
- Small (10K-100K)
- Medium (100K-500K)
- Large (500K+)

The correlation plots generated from our results for each of these categories above, as well as for all cities, can be found in [this folder](https://github.com/JimiLab/LocalifyMusicEventData/tree/main/LocalifyMusicEvents-USA-2019/figures).

We also have a full dataset consisting of 1246 cities with all population sizes, which can be found [here](https://github.com/JimiLab/LocalifyMusicEventData/blob/main/LocalifyMusicEvents-USA-2019/data/LocalifyMusicEvents-USA-2019_full.csv).

## Usage Instructions

1) Clone this repository: ```git clone https://github.com/JimiLab/LocalifyMusicEventData.git```. 

2) To reproduce our results used in the paper, run the notebook ```LocalifyMusicEvents-USA-2019/LocalifyMusicEvents-USA-2019_Step1_StatistcalAnalysis.ipynb```.

**IMPORTANT note for reproducibility:** Only run ```LocalifyMusicEvents-USA-2019/LocalifyMusicEvents-USA-2019_Step0_DataCreation.ipynb``` if you intend to use the **LATEST** data from CensusReporter. Do not run this notebook if you intend to reproduce our data and results. The dataset used in our paper can be found [here](https://github.com/JimiLab/LocalifyMusicEventData/blob/main/LocalifyMusicEvents-USA-2019/data/LocalifyMusicEvents-USA-2019_paper.csv). 


## Demo Poster

Demo poster presented in NEMISIG 2022 (Newark, NJ):

<img width="1197" alt="Screen Shot 2022-07-19 at 5 53 23 PM" src="https://user-images.githubusercontent.com/19521672/179855100-a532e248-3af1-4fd3-bc7a-a90b04b26783.png">


## License
This library is released under the terms of the MIT license. Full details in ```LICENSE``` file.
