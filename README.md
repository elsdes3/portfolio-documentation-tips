# Analysis of Bikeshare Usage in the Metro DC Area

This repository contains materials to support a talk about data science portfolio project organization and documentation. Analysis in this repository is not complete.

## [Table of Contents](#table-of-contents)
1. [About](#about)
   - [Background](#background)
   - [Data](#data)
   - [Objectives](#objectives)
2. [Requirements](#requirements)
3. [Usage](#usage)
4. [Project Organization](#project-organization)

## [About](#about)
### [Background](#background)
[Capital Bikeshare](https://www.capitalbikeshare.com/) is the bikeshare service for the Metro DC area in the US and covers jurisdictions including Washington, DC and Arlington, VA among others. Users can use the service for short trips around an area serviced by any of the more than 600 stations across these jurisdictions. Capital Bikeshare is [operated by Lyft](https://www.lyft.com/bikes/washington-dc).

### [Data](#data)
[Bikeshare ridership data (number of trips departing from each bikeshare station) is made available](https://www.capitalbikeshare.com/system-data) for every trip taken using this bikeshare service. We will use this to extract insights about how the service.

Raw system data will be retrieved directly from the Capital Bikeshare public webpage, processed and then used in the quantitative analysis.

### [Objectives](#objectives)
In this project, the bikeshare ridership data will be used to develop a ML model to predict bikeshare departures per station to be used by the bikeshare operator to [rebalance bikeshare stations](https://builtin.com/data-science/bike-share-rebalancing).

## [Requirements](#requirements)
This project requires the following
1. [Python 3.10.2](https://www.python.org/downloads/)
2. Google Chrome version 97.0.4692.71
3. [Google Chrome web driver version 97.0.4692.71](https://chromedriver.chromium.org/downloads)

## [Usage](#usage)
1. Download the Google Chrome web browser and the [webdriver for the same version of the browser](https://chromedriver.chromium.org/downloads).
2. Create Python virtual environment named `bikeshareenv` and install the Python requirements into it
   ```bash
   $ pip3 install -r requirements.txt
   ```
3. Start a local Jupyter Notebook server
   ```bash
   $ jupyter notebook
   ```
5. Install new Python libraries
   - add new libraries to `requirements.txt`
   - run the following
     ```bash
     $ pip3 install -r requirements.txt
     ```

## [Project Organization](#project-organization)

    ├── 01_dont_do_this.ipynb       <- Jupyter notebooks; naming convention is a prefix
    |                                  followed by a `-` delimiter and short description of
    |                                  the tasks performed in the notebook.
    ├── 02_get_data.ipynb
    ├── data
    │   ├── processed               <- prepared data, ready to use for quantitative analysis.
    │   └── raw                     <- raw data; should never be changed.
    ├── LICENSE
    ├── README.md                   <- README for developers to use this project.
    └── requirements.txt            <- Python requirements file
