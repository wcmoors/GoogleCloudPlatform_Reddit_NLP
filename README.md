# GoogleCloudPlatform_Reddit_NLP
Using Google's Compute Engine, Cloud Storage, NLP API, and an analytical database to process and interpret Reddit New feed sentiment.

Overall process and components used for the project.
--------------------------
Components:

A preemptable VM
GCP Bucket
GCP Postgres Instance
Python script to read in Reddit RSS feed to VM then load it to the GCP Bucket
Python analyze-entity-sentiment command to analyze the reddit data and write it to a json file
Overall Process:

After creating all of the components, I ran the python script to pull reddit rss feed data into the VM and load it to the GCP bucket.
Then I used the python analyze-entity-sentiment command to analyze the sentiment in the reddit data and write it to a file on the VM
Then I downloaded that file to my PC and uploaded it to the JupyterHub module8/exercises folder
Then I read the json file into a python dataframe and uploaded it to the GCP Postgres instance
Then I pulled the data from the postgres database into a python dataframe (just to demonstrate it can be done)
Then I wrangled the data a bit and created some basic visualizations
