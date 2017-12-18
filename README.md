# TxtLocViz
Visualizing Locations in text

## Overview

### This Flask application performs the following:
Input text from screen, file or website is processed using NLTK Stanford NER Tagger to identify and tag Locations.
The tagged locations are then chunked, in cases where the location is a multi word term (“New York City” for example).
This output is processed to produce an HTML file where locations are <mark>ed to create a visualization of locations highlighted in the text.
Each location is also sent to a geolocator that returns its coordinates. The coordinates are sent through Google maps API to produce a map with the locations pinned.


## Installing the application and dependencies

Download and install python 2.7 - https://www.python.org/downloads/

Install Flask - http://flask.pocoo.org/docs/0.12/installation/#installation

Install NLTK - http://www.nltk.org/install.html

Install Stanford NER Tagger - http://www.nltk.org/api/nltk.tag.html#nltk.tag.stanford.StanfordNERTagger

Install geopy - https://pypi.python.org/pypi/geopy

Get Google API key: https://developers.google.com/maps/documentation/javascript/get-api-key

Download the Txt_Loc_Viz application code from github <link>

Unzip into a folder

## Updates

Enter the directory where you installed tagger in step 4 into the parameter stanford_dir in the file Run27geo.py where marked

Enter the API key you obtained in step 6 into these files where marked: R_url.html, R_file.html, R_text.html

## Usage

Open terminal/command prompt

Navigate to the folder

Run the application
```bash
python Run27geo.py
```

In a browser go to: localhost:5000 to use the application
