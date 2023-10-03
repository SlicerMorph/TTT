# TTT
SlicerMorph Train the Trainers


## Generating Terminology to be used in Slicer

Go to https://github.com/Imageomics/slicerMorph_JSON_generator

Click green code button and choose download.

Unzip the zip file a folder (e.g., your desktop)

### MacOS
Open a terminal windows
type 
```
pwd
```
(this will indicate which folder you are currently in (print working directory)
then type 
```
/Applications/Slicer.app/Contents/MacOS/Slicer --no-splash --no-main-window --python-script "/Users/amaga/slicerMorph_JSON_generator-main/generate_slicer_json.py" "/Users/amaga/slicerMorph_JSON_generator-main/test.csv"
```

generated file will be under the folder indicated by the pwd command above.
### Windows

