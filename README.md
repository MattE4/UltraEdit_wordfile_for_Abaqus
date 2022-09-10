# UltraEdit wordfile for Abaqus FEA
Wordfile for editor UltraEdit that enables syntax highlighting, function list and code folding for the input file of Abaqus (FEA tool)

## Function List
- Works as planned
- Regex makes it easy to identify keywords
- Abaqus Keywords lines are shown in the function list
- Double-click on them allows to jump to the keyword


## Syntax Highlighting
- Works nearly as desired
- Regex can't be used for this
- Workaround for keywords is okay, but not perfect for all keywords
- Many parameters and parameter values are included, but not all of them
    - Not that important to me


## Code Folding
- Originally I planned to fold the big blocks of *Node and *Element
- I didn't achieved this, since te worfiles requires to define a beginning and end of the block
    - Abaqus has no end keyword for those options
- Now I've used to the parts and the assembly for folding
    - Uses *Part -> *End Part and *Assembly -> *End Assembly
- Takes some seconds to identify when opening a medium to large input file for the first time
    - Might require to hit F8 to update the parsing of UE