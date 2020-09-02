**What are the software requirements?**

1. Python IDE
2. Microsoft Excel

**Where to download the data?**

Nighttime light: [https://ladsweb.modaps.eosdis.nasa.gov/search/order/3/VNP46A1--5000/2020-02-01..2020-04-03/DB/World](https://ladsweb.modaps.eosdis.nasa.gov/search/order/3/VNP46A1--5000/2020-02-01..2020-04-03/DB/World)

Air Quality Index: [http://www.cnemc.cn/](http://www.cnemc.cn/)

**How to get the results?**

Run the below scripts to generate nighttime light and AQI data. Install required packages for the scripts.

1. VIIRS-VNP46A1.py

This script is used to calculate the daily nighttime light radiances for the entire target region. Change following variables accordingly.

    1. data\_infolder– root directory for input files
    2. utput\_dir – root directory for output files
    3. alldate – study period

1. dnb-monthly-VNP.py

This script is used to calculate the monthly mean of nighttime light over the target region. Change the following variables accordingly.

    1. input\_dir – root directory for input files
    2. utput\_dir – root directory for output files
    3. alldate – study period

1. dnb-difference-VNP.py

This script is used to calculate the difference of nighttime light between different months. Change the following variables accordingly.

    1. input\_dir – root directory for input files
    2. utput\_dir – root directory for output files
    3. region – study area
    4. pre\_nc\_filename – monthly mean of nighttime light in China during former month
    5. post\_nc\_filename – monthly mean of nighttime light in China during latter month

**Results**

1. NTL-2019.xlsx contains the monthly mean of nighttime light in all the provinces of mainland China in 2019.
2. Nighttime\_light\_data.xlsx contains monthly mean nighttime light of provinces and entire country of China.
3. AQI\_data.xlsx contains daily and monthly mean of AQI in provinces and entire country of China