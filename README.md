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
/Applications/Slicer.app/Contents/MacOS/Slicer --no-splash --no-main-window --python-script "/Users/amaga/Downloads/slicerMorph_JSON_generator-main/generate_slicer_json.py" "/Users/amaga/Downloads/slicerMorph_JSON_generator-main/test_data/terminology_test.csv"

```

this will output a file called **segmentation_category_type.json **in the folder indicated above. 

Open this file in the text editor, and change the first line from:

` "SegmentationCategoryTypeContextName": "Segmentation category and type"`
to
`  "SegmentationCategoryTypeContextName": "SlicerMorph category and type"`
then save. 
### Windows
TBD

### Slicer instructions

Open Slicer

Search for the terminology module, then click the little + sign on the right hand side

Navigate to the json file and choose that.

generated file will be under the folder indicated by the pwd command above.

