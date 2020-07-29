# Building Custom Discovery for Digitized Collections Using Computational Methods

By Scott Bailey

*Triangle Research Library Network (TRLN) Annual Meeting 2020*

Computational methods, such as topic modeling, create an opportunity for librarians to build experimental graphical interfaces to digitized collections. In this hands-on workshop with the Python programming language, participants will learn how to topic model a text corpus, and build interactive visualizations to expose items in the collection in new ways.

Throughout this workshop, we'll pay careful attention to the moments in our process where human and expert attention is still required. 

## Running the workshop code

All of the code in this workshop exists in Jupyter Notebooks (`.ipynb` files). The workshop code can be run in multiple ways. 

If you already have a local Python installation and are comfortable working with virtual environments, go ahead and create a virtual environment and install the libraries listed in `requirements.txt` in your preferred way. This workshop was developed with Python 3.8 (by way of `pyenv`) and `virtualenv` for simplicity, but you could use `conda`, `pipenv`, `poetry`, or other environment managers. 

If you are just getting started with Python or simply prefer to work in the browser (I recommend this for the live workshop), click on the Google Colab button below to open the workshop notebook in Google Colab, Google's hosted Jupyter Notebook environment. You'll be able to run all of the code in your browser. 

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/csbailey5t/TRLN-Workshop-2020/blob/master/model-visualize.ipynb)

You can also run the full notebook in Binder. To run in Binder, click the button below:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/csbailey5t/TRLN-Workshop-2020/master)

## Our Corpus: *The Animal Turn*

The digitized collection we'll work with today is from NC State University Libraries' Special Collections: *[The Animal Turn](https://www.lib.ncsu.edu/animal-turn)*. This is a grant-funded collection with substantial materials from NC State University Libraries' Animal Rights and Welfare collections, along with materials from the ASPCA's archives. We're only going to be working with the text of these materials today, but one could certainly use computational methods to explore the collection as images. 

This collection is backed by [IIIF (International Image Interoperability Project)](https://iiif.io/) and includes OCR text. With permission, I've taken advantage of the IIIF manifest for the collection, and scraped the OCR text. The scraping text is included in this repo in `scrape.ipynb`. 


## Resources on Machine Learning and Libraries

There is an ever-growing number of reports, articles, and environmental scans on the future of machine learning/artificial intelligence and libraries. Here are a select few pieces:

- [Responsible Operations: Data Science, Machine Learning, and AI in Libraries](https://www.oclc.org/research/publications/2019/oclcresearch-responsible-operations-data-science-machine-learning-ai.html) by Thomas Padilla
- [Machine Learning + Libraries: A Report on the State of the Field](https://labs.loc.gov/static/labs/work/reports/Cordell-LOC-ML-report.pdf?loclr=blogsig) from LC Labs and written by Ryan Cordell. 
- [Mapping the Current Landscape of Research Library Engagement with Emerging Technologies in Research and Learning](https://www.arl.org/resources/mapping-the-current-landscape-of-research-library-engagement-with-emerging-technologies-in-research-and-learning/) from ARL, CNI, and Educause. This isn't specifically and only about ML in libraries, but it's a heavy and recurring theme. 
- [Shifting to Data Savvy: The Future of Data Science in Libraries](http://d-scholarship.pitt.edu/33891/1/Shifting%20to%20Data%20Savvy.pdf), an IMLS funded report on libraries, librarians and data science. 


## Credits

This workshop is based off of work I did while at Stanford Libraries as part of the SUL AI Studio, a library initiative initiated to explore possible uses of machine learning/artificial intelligence in relation to library collections and services. Working with [Javier de la Rosa](https://www.linkedin.com/in/versae/), [Rebecca Wingfield](https://library.stanford.edu/people/wingfiel), and [Arcadia Falcone](https://library.stanford.edu/people/arcadia) on the [Jarndyce Single Volume Nineteenth Century Novel Collection](https://searchworks.stanford.edu/catalog?f%5Bcollection%5D%5B%5D=jt466yc7169), I experimented with different machine learning approaches to produce semantic models and cluster documents with an eye toward metadata creation and discovery. Code from that experimental, proof-of-concept only work is [here](https://github.com/sul-cidr/jarndyce).

This workshop builds directly from that work and would not have been possible without our great project team. 