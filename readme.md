This project contains scripts used to build an experiment with data on the Nara Rolls site. 

The process is something like this:
 - First, get images into notebooks/data/full
 - Second, extract text from images using tesseract
 - Third, use tesseract data and images to extract text again, this time with chatgpt, with much better results (see blog post)
 - Fourth, translate original German text to English, using chatgpt
 - Fifth - play around with different retrieval/search techniques

Note, these notebooks have not been run in this environment and may need some massaging to get going. I'm moving them here from another project. Also note, how there's a chdir command at the start of every notebook. For some reason that was the only way I could get it to work in intellij, since the starting directory always seems to be system root. You will need to modify that, depending on the project location.


Before you start, set environment variable 'export PIPENV_VENV_IN_PROJECT=1' (and maybe 'export PIPENV_IGNORE_VIRTUALENVS=1') and run 'pipenv install'.

To run chatgpt code, need .env file with a line "OPENAI_API_KEY="


