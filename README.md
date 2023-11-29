# PLP1: Introduction to R

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

## Naming Conventions 
- R is a case sensitive language; this means that `tree` and `Tree` are different variables, as are `my_Data` and `my_data`.
- Variable and function names are typically lowercaseper language conventions, however, they do not have to start with lowercase letters to be considered syntactically correct.
- Multi-word variables should be separated with an underscore: `my_data`. 
- Spaces should be placed around most infix operators and function calls with the exception of `:`, `::`, and `:::`.
- File names should be clear, concise and end in “.R”. If files need to be run sequentially, they should be named with numbers at the beginning: “_1-my_data.R_”, “_2-my_data.R_”  


## Data Types and examples   
-  **Integers**: The Integer function must be evoked to declare an Integer in R: `q = as.integer(6)`
    - To determine whether something is an integer: `is.integer(q)`
- **Character Data: R's version of Strings**: There are multiple ways to create a string in R.
    - Use double quotations: `my_string <- "New String!"`
    - Use single quotations: `my_string <- 'New String!'`
    - Make an empty string: `my_string <- ""`
    - Make an empty character vector: `ch_vr <- character(0)
- **Floating Point Numbers**:
    - xxxxxxxxxx
- **Vectors, Arrays and Lists**:
    - **Vectors** are a one-dimensional list and can contain only one data type. Some examples of creating vectors:
        - `vector1 <- c(1, 2, 3)`
        - `vector2 <-  c(10, 20, 30)`
        - `vector3 <-  c(“abc”, “def”, “gh”)`
    - **Arrays** are vectors in R that can have multiple dimensions, but can still contain only one data type.
        - To create a two-dimensional array (using the vectors created above): `array1 <- array(c(vector1, vector2), dim <- c(3,2,2))`
    - **Lists** are structures that can contain multiple data types in R; they can also contain other data structures such as vectors and arrays.
        - list1 <- `list(vector1, array1, vector2, 6)`
- **Dictionaries and Hashmaps**:
    - **Dictionary Equivalent**: The List structure is used to create the equivalent of a dictionary in R, but “keys” can be assigned to list items so we can index to them. Example:
        - `plants <- c("desert"="cactus", "mountain"="fern", "tropical"="lime tree")`
        - adding new pairs to a list dictionary: `plants["sea"] <- "seaweed"`

## General Discussion  
- R has 21 **keywords**, meaning these words are reserved and cannot be used for naming. Here's a few examples:
    - `if`, `else`, `while`, `for`, `break`, `next`, `repeat`,` NULL`, `TRUE`, `function`, `Inf`, `NA`, `in`, `NaN`
- R has very loose **naming rules**, and variables can be named close to anything. See "naming conventions" above, however, for stylistic tips.
    - Variable names must begin with a letter and can utilize letters, numbers, the dot character(`.`) and underscore(`_`).
    - Variables cannot begin with numbers or an underscore, but they can start with alphabet letters or a dot character: `.my_data`
    - If the name begins with a dot character, it may not be followed by a number
    - Variable names cannot use reserved words.
- R is **strongly typed**, meaning that certain operations cannot be performed between mixed data types.
- R is **dynamically typed**, meaning no variable type declaration is required when writing code.
    - It is also **implicitly typed**, meaning the language is able to deduce some data types based on context and use. Implicitly typed languages are always dynamically typed.
- R is **interpreted** rather than compiled.
- Most data types are **immutable** in R, meaning they cannot be modified after creation. Environments, symbols, specials and builtins are mutable in R . 
    - It's important to note that data frames are not mutable in R.
    - Some data types appear to be mutable, but R simply makes a new copy.
- R has 5 categories for **operators**: 
    - _Arithmetic operators_: for numeric values such as `int`, `float` and `double`.
        - `+`, `-`, `*`, `/`,` ^`, `%%`, `%/%`
        - These perform simple arithmetic operations. 
    - _Assignment operators_: Used to assign a value to a variable
        - `<-`, `=`, `<<-`, `->>` (
        - The first two operators assign a variable into the environment. `<-` can be used anywhere, and is more widely used in R. `=` Possesses restrictions.
        - the latter two are usually used only in functions, and can redefine a pre-assigned value. 
    - _Comparison operators_: used to compare numeric values
        - `==`, `!=`, `>`, `<`, `<=`, `>=`
    - _Logical operators_: for the combination of conditional statements
        - `&`(AND), `&&`(AND), `|`(OR), `||`(OR), `!`(NOT)
    - _Miscellaneous operators_:
        - `:`(sequence numbers), `%in%`(test whether element is in a vector), `%*%`(multiply matrices)


## Resources for Learning and Using R
1. [Official Documentation](https://www.r-project.org/other-docs.html)
2. [RStudio Education](https://education.rstudio.com/learn/beginner/)
3. [Getting Help with R](https://www.r-project.org/help.html)
4. [Burns Statistics: Impatient R](https://www.burns-stat.com/documents/tutorials/impatient-r/)
   
## Sources
1. [r-project.org/about](https://www.r-project.org/about.html)
2. [Posit](https://posit.co/)
3. [Princeton Research Computing](https://researchcomputing.princeton.edu/education/external-online-resources/R)
