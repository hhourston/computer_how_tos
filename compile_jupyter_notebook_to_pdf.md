# Preparing jupyter notebooks for conversion to pdf via Latex
Mon. Feb. 10, 2025

To convert a jupyter notebook file to pdf:
* Make sure xelatex installed and exported to PATH variable
    * https://stackoverflow.com/questions/52300242/solving-500-internal-server-error-nbconvert-failed-xelatex-not-found-in-path 
* You can also convert to pdf via HTML, but this was the method for converting via Latex

To format a jupyter notebook for conversion via Latex to pdf:
* Can hide code chunks and only show output
    * Link: https://stackoverflow.com/questions/49907455/hide-code-when-exporting-jupyter-notebook-to-html
    * Hide all chunks when exporting to pdf on command line, or go into the metadata for certain chunks in Jupyter to add tags to hide the chunks
    * Good for assignments when you don't need to show all your code
* Can remove heading numbers that are automatically added, by appending " {-}" to each heading name 
    * Link: https://stackoverflow.com/questions/35077571/how-to-remove-heading-numbers-in-jupyter-during-pdf-conversion
* Add title instead of using the file name as the title by adding a title field to the Notebook metadata
    * Link to online resource the same as for adding "authors"
* Add "authors" field to the Notebook metadata
    * Link: https://github.com/jupyter/nbconvert/issues/249
    * Make sure to use list-like format for authors value otherwise it doesn't work, even if just one author
    * When editing Notebook metadata, make sure to click the checkmark that appears after making your changes, otherwise changes aren't saved. If the checkmark doesn't appear and the Notebook metadata window is red, then there is an error in the code you added (such as a missing or hanging comma)
