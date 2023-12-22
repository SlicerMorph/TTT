# TTT
SlicerMorph Train the Trainers

## Github Instructions
Google docs: https://docs.google.com/document/d/1nlqBMseK-kWcCzIhsjqddkaBh3hEqlPWAU2TLoIztRA/edit?pli=1


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

` "SegmentationCategoryTypeContextName": "SlicerMorph category and type"`
then save. 
### Windows
TBD

### Slicer instructions

Open Slicer

Search for the terminology module, then click the little + sign on the right hand side

Navigate to the json file and choose that.

generated file will be under the folder indicated by the pwd command above.

## Forking and making changes in Slicermorph Tutorials
fork on web
```
git clone https://github.com/smrolfe/Tutorials.git
cd Tutorials
git checkout -b myTutorialUpdate
```
make some changes
```
git add .
git commit -m "Fix typo in GPA documentation"
git push git@github.com:YOUR_GITHUB_USER/Tutorials
```
create pull request from web
sync:
```
git checkout master
push to master
git push origin master
```
## Tutorials from the workshop
* [SPHARM Tutorial by Stephanie Smith](https://github.com/scutisorex/SPHARMtutorial)
* [ImageStacks and Visualization by Natalia Taft](https://github.com/Natalia-Taft/TaftTutorials)
* [Jaimi Gray's Segmentation Color Codes and Terms](https://docs.google.com/spreadsheets/d/1iVs6OMvu91sXPBWGYoZc6bKw9uy9J9e-z0Xs7ayfKRQ/edit#gid=0)
* [Dominick Dickerson: Using ImageStacks, Segmentation and SplitVolume to separate a full scan into subvolumes:](https://github.com/ddickerson31/TTTTutorial)
* [Susan Perrine: Segmentation Tutorial](https://github.com/SPerrine/3DSlicer_Segmentation_Tutorial)

