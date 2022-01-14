# Analysis of Bikeshare Usage in the Metro DC Area

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
[Ridership data is made available](https://www.capitalbikeshare.com/system-data) for every trip taken using this bikeshare service. We will use this to extract insights about how the service.

### [Objectives](#objectives)
In this project, the bikeshare ridership data will be used to perform _____.

Raw system data will be retrieved directly from the Capital Bikeshare public webpage, processed and then used in the quantitative analysis.

## [Requirements](#requirements)
This project requires the following
1. Python 3
2. Google Chrome
3. Google Chrome web driver

## [Usage](#usage)
1. Download the Google Chrome web browser and the [webdriver for the same version of the browser](https://chromedriver.chromium.org/downloads).
2. Create Python virtual environment named `bikeshareenv` and install the Python requirements into it
   ```bash
   $ python3 -m venv bikeshareenv
   $ source bikeshareenv/bin/activate
   $ pip3 install -r requirements.txt
   $ deactivate
   ```
3. Start a local Jupyter Notebook server in the `bikeshareenv` Python virtual environment
   ```bash
   $ source bikeshareenv/bin/activate
   $ jupyter notebook
   ```
4. Deactivate the virtual environment
   ```bash
   $ deactivate
   ```
5. Install new Python libraries into the `bikeshareenv` Python virtual environment
   - add new libraries to `requirements.txt`
   - run the following
     ```bash
     $ source bikeshareenv/bin/activate
     $ pip3 install -r requirements.txt
     $ deactivate
     ```

## [Project Organization](#project-organization)

    ├── 01_dont_do_this.ipynb       <- Jupyter notebooks; naming convention is a prefix
    |                                  followed by a `-` delimiter and short description of
    |                                  the tasks performed in the notebook.
    ├── 02_get_data.ipynb
    ├── data
    │   ├── processed               <- prepared data, ready to use for quantitative analysis.
    │   └── raw                     <- raw data; should never be changed.
    ├── install_requirements.sh     <- script to install all Python requirements
    ├── LICENSE
    ├── README.md                   <- README for developers to use this project.
    └── requirements.txt            <- Python requirements file
