# LFWriteAssist

This repository contains resources for the paper "LanguageTool as a CAT tool for Easy-to-Read in Spanish". 

# Installation guide for the LFWriteAssist

STEP 1:
- Visit the page: https://www.python.org/downloads/ and download the latest Python version.      	
- If you are not familiar with Python and/or do not use it regularly, install the appropriate version according to the default settings of the installation. Make a note of the installation path.  
- "Add python to PATH" should be ticked during the installation.

STEP 2: 
- Unpack the zip archive.
- Install the requirements: "pip install language_tool_python spacy sumy nltk compound-split" and - "python -m spacy download es_core_news_sm".

STEP 3:
- You must replace the grammar.xml file in LanguageTool
- You need to go to the directory where you installed Python.
- Go to the subdirectory: <Python_directory>\Lib\site-packages\language-tool-python\[LanguageTool Version]\org\languagetool\rules\es
- On most Windows systems, you can use this path: C:\Users\[User of the PC]\AppData\Local\Programs\Python\[Pythonversion]\Lib\site-packages\language-tool-python\[LanguageTool Version]\org\languagetool\rules\es
- Copy the grammar.xml from the zip file into the above subdirectory and overwrite the grammar.xml file there.
- Sometimes, a .cache hidden folder is automatically created for LanguageTool. In these cases, the rules must be changed here: /Users/[User of the PC]/.cache/language_tool_python/[LanguageTool Version]/org/languagetool/rules

STEP 4:
- Execute LFWriteAssist
- Execute the lfwriteassist.py script: "python LanguageApp.py".
- A window will now open, indicating that the installation has been successfully completed.


# How to use LFWriteAssist
The structure of the interface consists of the following parts: 

- Input panel, named "Campo de entrada", which is a text entry field where users write their source text. 
- The second panel, named "Resumido y revisado", shows the summarized text, the tool's suggestions on the original text (both for automatically corrected parts, and areas that need revision), as well as definitions of complex, polysemic, or infrequently used terms, acronym expansions, and easier synonyms. 
- The third panel, named "Resumido y corregido automáticamente", shows the summarized and automatically corrected version of the source text. Those parts of the text that have been automatically corrected are underlined in green. Those parts underlined in orange are parts of the text that violate some LF rule, but have not been automatically corrected. 
- The side panel, named "Lista de normas", lists the rules for LF that we have created. 
- The slider control, named "Longitud del resumen en %", allows the user to adjust the length of the summary. When choosing 100%, the output text will keep all the information in the source text.


STEP 1: 
- Here, you have to copy paste your original text, in the panel "Campo de entrada" and then click on "Resumir y revisar" 

