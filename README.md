# Identifying Communal Microblogs during Disaster Events
The huge amount of tweets posted during a disaster event include information about the present situation as well as the emotions / opinions of the masses. While looking through these tweets we realized that a large amount of communal tweets i.e., abusive posts targeting specific religious / racial groups are posted even during natural disasters. Considering the potentially adverse effects of communal tweets during disasters, in this work, we develop a classifier to distinguish communal tweets from non-communal ones. We also propose an event-independent classifier to automatically identify anti-communal tweets which can be utilized to counter communal content during disasters. This classifier was proposed in the following paper:

CITE PAPER HERE

The classifier can also be tested at the following link: http://cnerg.iitkgp.ac.in/p/disaster-helper/dishelper/communal-identifier.html

The repository contains the code and dictionaries needed to run our classifier.


## Prerequisites

For using this classifier, you will need Python2 with [nltk](www.nltk.org) installed.


## Running the Classifier

Use the file [Communal_Tweet_Classifier.py](Communal_Tweet_Classifier.py) present in the root directory of this repository for using our classifier. The script takes 2 command line arguments as input - input file path and output file path. Input file should contain one tweet in each line. Output file contains 3 columns (tab-separated): tweet and the predicted class (1, 2 or 3). 1 is for communal, 2 for non-communal and 3 is for anti-communal. Please provide only disaster-related tweets as input. Sample run:
```
 python Communal_Tweet_Classifier.py Sample_Data/sample_input.txt Sample_Data/sample_out.txt
```