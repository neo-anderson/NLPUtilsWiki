NLPUtilsWiki
============
Wiki source until the main repository becomes public

## What's New

**Version 1.0**
- UI Changes. Widened the composite groups and expanded the textboxes
- SVM - error messages if input/output paths are not selected
- SVM - Crossvalidation before separate test datat
- SVM - Remove wordcount - tfidf default
- SVM - feature weights - checkbox, directory change to output dir
- SVM - output folder, not output file. create csv, weights and svm output files in the output folder
- Naive Bayes - GUI like SVM. Tabs for test and classify modes
- Naive Bayes - Made 'Keep sequence' false by default. Removed option from GUI.
- Naive Bayes - Restructured.
- Naive Bayes - Removed Preprocessing plugin as mallet does not have manual label input
- Naive Bayes - Added checkboxes for case conversion and removing stop words
- Naive Bayes - Added Classification report output
- Naive Bayes - Accuracy output to console log
- Naive Bayes - added CSV output
- Naive Bayes - fixed directory dialog buttons
- Ran Senate Crawler and extracted the entire 113 congress senator records.

**Version 0.9**
- New Options - All Senators, All Republicans, All Democrats, All Independents
- New method of filtering relevant links
- Check box for "limit records per senator"
- Fixed Welcome page - auto resize
- Fixed buttons in Mac.
- Crawler can search with date range, congress number, senator name, limit maximum number of records for each senator, or with just the senator name - search all congresses and dates. Can also search a particular senator of a specific congress only
- dynamically gets a list of congresses n corresponding senators for the user to choose.
- Loops over all the available congresses
- Repeatedly searches congressional record for each senator present during the congress.
- Extracts the selected senator's dialogue. Continue extraction of dialogues spanning multiple lines until the dialogue of the next speaker.  
- Added a feature to limit the maximum documents per senator
- Format output filenames based on template

**Version 0.8**
- Created Senator Crawler plugin 
- Outputs CSV file with name congressnum-senatorname-party-state-date-title.txt
- Extracts only the dialogues by the selected senator.
- Removed plugin menu

**Version 0.7**
- Created Basic ZLabelLDA plugin
- Linear Kernel made default for SVM. Removed option from UI.
- Pretrained options disabled unless checkbox selected.
- Changed icon and splash screen
- Created Preprocessing pop up plugin
- LDA Output - csv file support added. Also, prefix added based on the directory or manually provided
- LDA - added word count output

**Version 0.6**
- Added Linear Kernel to the SVM Classifier (Faster, More Accurate for Text Classification, Provides weights - required to calculate predictive weights)
- Calculate Predictive Weights if Linear Kernel and not doing Cross Validation.
- Added LDA plugin
- New Menu item for Topic Modelling
- Added Word Weights output and Dirichlet parameter
- Added NBClassifier
- Instructions to wiki
- Mac OS X Testing and bug fixes
- Removed error log section
- Removed predictive weights plugin
- New menu for Wordcount plugins
- Changed utilities menu label to Basic Tools
- Branding - Splashscreen, Title USC NLPUtils, 32x32 gif Icon with USC Colours and USC Font.

**Version 0.5**
- SVM Classifier
- Added preprocessing options to the classifier
- csv output
- TF and TFIDF methods for training.
- Load pretrained models
- k-fold Cross validation
- Predictive Weights plugin

**Version 0.4**
- Created preprocessing plugin with features like removing special characters, converting to lowercase, removing stopwords and stemming.
- Stemming now has a language option. It is set to Auto Detect by default and will detect the language of each input file individually and choose the appropriate stemmer algorithm. The user can also manually select the language of the files.
- Fixed the console log. Now all the plugins can update the context and the console log will pick up the changes and display to the user.
- Fixed return code bug: return code gets overwritten and hence the last error message keeps getting displayed. Fixed

**Version 0.3**

Added a Welcome Page, which informs the user about the latest version and the changes.<br/>
Removed Sample demo parts from the GUI.<br/>
Added Porter 2 stemming option.<br/>
Made LIWC-style Stemming optional<br/>
Added SPSS Raw Data Output Format.<br/>
Added option to calculate Category-wise Word Distribution for each file.<br/>
Added Word Count (WC), Average Words per Sentence (WPS)and Percentage of words longer than 6 letters (Sixltr) to the output features.<br/>
Modified Percentage calculation of categories based on LIWC<br/>
Category Count now counts total words and not unique words.<br/>
Added Basic Weka NaiveBayes Classifier Implementation<br/>
Modified the Plugin menu with placeholders for adding/removing plugins and setting global options.<br/>
Added Utilities Menu for Wordcount plugin and Classifiers menu for classifier plugins<br/>
Fixed Package Names and Build Errors<br/>
Created github repository and committed the code<br/>

