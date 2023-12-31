# The Coder's Computer

## Choosing a Text editor

# It is important to remember a few things when choosing a text editor!
- They are essentially the same but with different text editing software, varying on the software
- Whichever you prefer and gets the job done is fine!
  
# The Most Important Features in a Text Editor
- Code Completion
- Suggests code to complete your line of code, saving you time by providing a choice, so you don't finish typing and make typos
- Emmet: Shorthand (HTML and CSS) language extension to speed up your code writing. (Some text editors come with emmet built in, but can be installed via extension)
  
# Syntax Highlighting
* Will auto highlight different areas with color so you can differentiate your code for reference  
* Theme Variety (To reduce fatigue & eye strain)
* Can change the background & font colors to help you in your working environment
*  The ultimate goal is to reduce strain on the eyes
* A set of extensions readily available to be downloaded
* The ability to add features to your editor will be handy
  
> Text editors that come pre-installed on your computer usually lack the necessary components above. However, if you decide to use these pre-installed programs, make sure your machine does the following:
- Creates plain text code. No options for bold, italics, underlined, etc should be seen here
- Structure of files should be organized by the user (you), Be sure to save all files in the appropriate folders/subfolders!
- Double check your extensions
- Double check your written code! No completed code will result in typos that need to be double checked!
  
# Third-Party Options
* Notepad ++
* **ONLY** Windows Machines
* Syntax Highlighting, Code & Word completion, Function Completion
* Zoom
* Searchable Wiki, Online Community, & Chatroom

# TextWrangler (BB Edit)
+ Paid features but a 30D trial is available
+ For more, [Click](https://www.barebones.com/products/textwrangler/)

# Visual Studio Code
+ Free from Microsoft
+ All platforms
+ Emmett included for HTML & CSS
+ Syntax Highlighting, Extensions, Themes, Code Completion
+ Large Following

# Atom
- Free from Github
- All platforms
- Syntax Highlighting, Themes, Extensions
- Highly recommended
  
# Brackets
 - Free from Adobe
 - All platforms
 - **ONLY** Supports HTML, CSS, JavaScript without extensions, which can be downloaded.
 - Live Preview


# Sublime Text 3
- Free Version
- Premium Version ($70)
- Everything Included


# Difference between Text Editors & IDE
- IDE's contain text editors, but piled in with other software (File manager, complier, and a debugger)
- May be overwhelming for beginners


# Text Editors Conclusion
- Text editors change often, keep up to date with the latest software updates, so your experience is efficient for you


# Linux Tutorial
Line One
1. Prompt - Example: > `~`
2. Command - Example: > `ls`
3. Argument or Option typically starts with a dash. Example: > `-1`
4. Argument
> Spaces have to be between each of the 4


# The Shell: Bash
- The shell is the part of the OS (Operating System) that defines how the terminal will act and appear after typing in a command. Most Common shell is known as `Bash.`
- Use the command `echo $SHELL` to find out which shell you are on.


  # How to move
   `PWD`
  - "Print Working Directory"
  - Will tell you the current location within the directory


  `ls`
  - "List"
  - Gives you a list of the files available in your current location
  - Adding > `-1`, will give you more information about the files. It will show the type of file it is, Permissions, Blocks, Owner, Group, or directory it belongs to, size, modification time, name, or directory
  - Adding > `l -1/etc` , you can see the list of the contents on that directory

 
# Paths
   
  i. Absolute
- Specifies a location in the file or directory in relation to the root directory
- Always begins with (/) 
 `I.E (/home/mochi/documents/file.txt)`
      
 ii. Relative
 
  Specifies a location in relation to where you are sitting in the system
      - Will not begin with (/)
      - `Example: ls documents file.text`


### Paths continued: Shortcuts
       1. ~ (tilde) - represents shortcut for home directory
       2. . (dot) - represents the current directory
       3. . . (dotdot) - represents the parent directory

CD (Change Directory)

    1. cd can be ran without any arguments to take you back to home directory
    2. cd is usually ran with a single command line argument to show where you want to go
    3. The location can be specified as "absolute or relative" path    
    Tab can be used to completed the command line, ONLY if there is a possible outcome

  `mkdir` (make directory)
  
    - Alternative to right clicking a folder to create a new folder

  `touch` (create a new file)
  
  - Alternative to left clicking a folder to create a new folder


# Four important features to look for in a text editor?
           + Code Completion
           + Syntax Highlighting
           + Theme
           + Extensions
             
## Commands & their outcomes
      - PWD- Print Working Document, will show your current location in terminal
      - ls - List, shows you a list of files in your current location
      - cd - Change Directory, takes you to the file or directory you choose. Just stating `cd` will return you to the home directory.
      - mkdir - Make Directory, creates new file
      - touch - Creates new file
      
# Scenarios

 1. CD projects - Changing location in terminal to folder "projects"
 2. mkdir new-project - Create new folder/directory in "projects" folder
 3. touch new-project/newfile.md - User is creating a new file in "new-project" folder
 4. cd . . - return to parent directory of "projects"
 5. ls projects/new-project - ask for a list of files in "new-project" folder that is in the parent directory "projects"
