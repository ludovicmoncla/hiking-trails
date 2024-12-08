# Hiking trails


The repository contains a raw dataset of hiking trails (in France) crawled from the website [www.visorando.com](https://www.visorando.com). The dataset is in French and contains the following files: [TXT](./data/visorando-2013/txt) and [GPX](./data/visorando-2013/gpx).

The dataset was crawled in 2013 and contains 1,540 hiking trails. It has been used in the [Perdido](https://github.com/ludovicmoncla/perdido) and [CHOUCAS](https://choucas.ign.fr) projects.

* [geocoding.ipynb](./geocoding.ipynb): This jupyter notebook shows how to geocode the hiking trails:
    - compute a bounding box for each trail based on the GPS track.
    - geoparsing (NER + geocoding) with the [Perdido](https://github.com/ludovicmoncla/perdido) library. It uses Nominatim (OpenStreetMap) as a geocoding service.
    - NER with the [spaCy](https://spacy.io) library and geocoding with the [Perdido](https://github.com/ludovicmoncla/perdido) library. It uses Nominatim (OpenStreetMap) as a geocoding service.
    - NER with the [spaCy](https://spacy.io) library and geocoding with the [geocoder](https://geocoder.readthedocs.io/providers/GeoNames.html) library. It uses the [GeoNames](https://www.geonames.org) geocoding service.
