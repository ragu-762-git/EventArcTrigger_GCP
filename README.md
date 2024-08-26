# EventArcTrigger_GCP
This repository contain files for executing event arc trigger when a JSON(Newline delimited file) hits a cloud storage bucket

When a file with JSON (Newline Delimited) format hits a GCS bucket, the event arc trigger executes the cloud function.
The YAML file contains the list of possible schemas for the fixed JSON (Newline Delimited) format. Every time, when a file hits the bucket, the schema of the arrived file is matched with the list of schemas in the YAML file. If the schema matches. the data in the file will be written (overwrite) to the Big Query table. 
