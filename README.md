# python-playwright setup
how to setup python playwright project in your MacOS, but you can use this guide to start a general purpose python project as well. 

## Prequisite 
You should already have python3 install in your computer, if not, go to [python.org](https://www.python.org/) to learn more.

or go find your current version of python. Usually in /Library/Frameworks/Python.framework/Versions/3.10/bin/python3


## 1. Create your project folder. 
```commandline
mkdir playwright-demo
cd playwright-demo
pwd
```

## 2. install virtualenv. Learn more [here](https://learnpython.com/blog/how-to-use-virtualenv-python/)
```commandline
# install or upgrade your pip version
/Library/Frameworks/Python.framework/Versions/3.10/bin/python3 -m pip install --upgrade pip
# check your version
pip --version
# install virtualenv library
/Library/Frameworks/Python.framework/Versions/Current/bin/pip3 install virtualenv
```

## 3. create a virtualenv within your project
```commandline
# go to your playwright-demo folder and create a virtualenv venv folder
/Library/Frameworks/Python.framework/Versions/3.10/bin/python3 -m venv venv
# to activate your virtualenv
source venv/bin/activate
# to check your virtualenv is activated, whereis python will show you that you will be using python inside your venv folder
whereis python
```

## 4. install libraries to your virtualenv 
- Here i am installing for playwright, pytest , yaml. But you can setup your library for your own python project.
```commandline
pip install pytest-playwright
pip install pytest-xdist
pip install pyyaml
```

## 5. install playwright browser
```commandline
playwright install
```

## 6. test out playwright 
go to [Add Example Test section](https://playwright.dev/python/docs/intro#add-example-test)
```commandline
# run the playwright script
pytest
```

## 7. store your project to git
download [github desktop](https://desktop.github.com/)
> File > Add local repository > enter your project url and follow instruction

## 8. checkin a ReadMe.md file in your project 
```commandline
cd playwright-demo
touch ReadMe.md
```
- Open the ReadMe.md
- Type something into ReadMe.md
- save the file
- go to your github desktop
- you should see 1 change in ReadMe.md. type in the summary and description. Press "Commit to main" to save into your repository.
- go to github.com 's project folder and see if your changes made it to your live repository.



