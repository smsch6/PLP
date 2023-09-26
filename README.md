# Introduction to R

## History 
The name of this language is R, derived from its predecessor S. R was created by statisticians Robert Gentleman and Ross Ihaka at the University of New Zealand, Auckland. It was developed to address the lack of accessibility to statistical software, specifically the language of S, which was developed in Bell Laboratories as statistical analysis software but became monetized and restricted. R is open-source and free to use unlike its predecessor. R is used primarily for statistical analysis and machine learning for data analysis. It is widely used in the fields of Data Science, Bioinformatics, Biostatistics and general data analysis. R has excellent documentation, and most information about the language, its syntax, and installation can be found [here](https://www.r-project.org/other-docs.html).

## Installation 
A simple and effective method of coding in R is through RStudio. RStudio allows users to write in R in a graphical interface, where everything necessary to code in R can be viewed in one window. Both R and RStudio must be installed, and R must be installed first. R can be written in VSCode and multiple other platforms, however, RStudio was created specifically for the language and is incredibly simple to use. 

### Installing R 
1. Open [r-project.org](https://www.r-project.org/) in an internet window. 
2. Under "Download" below the R logo, click on "CRAN". You'll have to choose a CRAN mirror, one of many servers that store identical and recent versions of R.
3. Choose any CRAN mirror located in the US, ideally one geographically close to your location. (Statlib from Carnegie Mellon University in Pittsburgh, PA works well for those located in the Northeastern US.)
4. After selecting a CRAN mirror, follow the Operating-System appropriate link under "Download and Install R".
5. Choose the download link appropriate to your Operating System and specific version under "Latest Release". This will download the R Package Installer to your computer.
7. Save this file (ending in .pkg), open in and follow installation instructions.


### Installing RStudio
1. Open [Posit](https://posit.co/) in an internet browser and click "Download RStudio".
2. Click "Download RStudio" under "RStudio IDE" to download the free, open-source version of RStudio.
3. You have already installed R, so skip to step 2 and click the download button for your specific operating system. This downloads the RStudio Installer to your computer.
4. For Mac Users, go to the app store and download "Xcode". Open the app and allow it access to anything it requests. This is an Integrated Development Environment that allows you to create software on a Mac.
5. Open the .dmg file you downloaded from [Posit](https://posit.co/download/rstudio-desktop/), open it and follow installation instructions.

## Getting Started: Writing and Running Code in R
1. Open RStudio. You will always open RStudio (rather than R itself) to write a program in R.
2. Create a new script: Click "File" > "New File" > "R Script". The R Script is where you will write your program in R.
3. Once this script is open, you will see an empty window in the top left. This is where you will write your code in R.
   - The "Environment" tab in the top right will display variable saved to your Global Environment.
   - Results of running your script will be displayed in the Console in the lower left corner.
   - "Files" in the bottom right window displays which files are currently imported and loaded into RStudio.
   - "Plots" in the bottom right window displays plots produced in your Script.
   - "Packages" in the bottom right window displays which packages are loaded. To install a new package necessary, search its name in the search bar.
4. To run your R Script, click "Run" in the top right. There are options in the drop-down menu to run a single line, a section, or the whole script.
5. To comment out a single line, type a single hashtag (#) before the code.
   - example: `# print("Hello World")`
6. To comment out an entire section of code, type "Ctrl + Shift + C" on Windows and "Command + Shift + C" on MacOS.
7. RStudio does not auto-save, so save often.

## Resources
1. [Official Documentation](https://www.r-project.org/other-docs.html)
2. [RStudio Education](https://education.rstudio.com/learn/beginner/)
3. [Burns Statistics: Impatient R](https://www.burns-stat.com/documents/tutorials/impatient-r/)

## Sources
1. [r-project.org/about](https://www.r-project.org/about.html)
2. [Posit](https://posit.co/)
3. [Princeton Research Computing](https://researchcomputing.princeton.edu/education/external-online-resources/R)https://researchcomputing.princeton.edu/education/external-online-resources/R
