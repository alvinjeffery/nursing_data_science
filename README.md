# 2018 Nursing Knowledge: Big Data Science Pre-Conference

## Data Science Tutorial

I highly recommend the following Jupyter Notebooks for learning data science skills in Python:
https://github.com/fonnesbeck/Bios8366/tree/master/notebooks

## Software Carpenty Link for Group

https://software-carpentry.org/lessons/


## Creating Synthetic Data
To create 10,000 patients from the state of Ohio and make reproducible (using a seed), run...  
`./run_synthea -s 123 -p 10000 Ohio`

Notably, I made the following changes to the `./src/main/resources/synthea.properties` file...
`
exporter.years_of_history = 5
exporter.fhir.export = false
exporter.fhir.use_shr_extensions = false
exporter.fhir_dstu2.export = false
exporter.hospital.fhir.export = false
exporter.hospital.fhir_dstu2.export = false
`
to reduce file size with all the FHIR files we don't need for the workshop.  

