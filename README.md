# Flask_test
test environments for flask


The code was developed with VisualStudioCode. The important considerations:
1) Install Python interpreter and other python related plugins.
2) Install Azure extension as well. 
3) To develop and bind any flask, it is important to create a new folder. Load your model.pkl file into this folder and a regression_model.py file as well. 
4) Create a virtual environment (super useful when writing the requirements.txt file). Code is python -m venv <<nameofvirenv>>  Activate the virtual environment - code is <<nameofvirenv>>\Scripts\activate
5) Install flask, numpy, pandas, sklearn and whatever files that are required for running the ipynb/py files. 
6) create your app.py file, template files (index.html and predict.html). 
7) Run your app.py file and check if the link works. Now create a requirements.txt file (pip freeze > requirements.txt)
8) As a last step, go to the folder and create a Procfile. The procfile has no extension so just create a text file, enter the following line: web: gunicorn app2:app    where app2 is the name of my app file that runs my flask commands and app is the name given at the end of the app2 code after if_name_main line. (***Important***)
9) Now go to your azure plugin and open app services - follow the step by step procedure that automatically appears to create a webapp. Just select resource, Linux base and python 3.6/3.7 for launching the app.
