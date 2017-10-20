
![PyData_logo](./images/pydata-logo-warsaw-2017.png)

## Friday Oct. 20, 2017 - 15:00–15:30 in Track 3
# [Analysing flight safety data with Python](https://pydata.org/warsaw2017/schedule/presentation/51/)

### JESÚS MARTOS CARRIZO, ALEJANDRO SÁEZ MOLLEJO
#### Audience level: Novice

## Description

Is aviation the safest means of transport? Is flying now safer than in the previous decades? Which are the main accident causes? During this talk we will try to answer these and other questions using the capabilities of libraries such as pandas, cartopy or Bokeh.

## Abstract

A continuous improvement in flight safety is a common goal for all public agencies and private companies. Many analysis are published every year but, would it be possible to reproduce those same results? During this talk a real open database from the American National Transportation Safety Board (NTSB) will be used in order to show to the audience the potential of Python to read, clean and manipulate data. Among other questions, we will try to identify the most common causes of aviation accidents and their consequences. During the talk the importance of open data will be highlighted.

---

### Getting the data

As the database is too big to be uploaded to the repository it is stored separately [here](https://www.dropbox.com/s/n9inalri0dvff1j/avall.db?dl=1). It can be placed in the `data` folder manually or downloaded using `flight_safety/get_data.py` python script.

The data can also be obtained directly from NTSB website (https://app.ntsb.gov/avdata/) in `mdb` format. In order to convert it to a SQLite database the script `export_access2csv.sh` in `utils` folder can be used:

```
$ bash utils/export_access2csv.sh data/raw/avall.mdb data
```

### Requirements

It is recommended to use Anaconda/miniconda (https://www.anaconda.com/download) to install the dependencies. After conda is installed, the environment.yml can be used:

```
$ conda env create -f environment.yml
```

