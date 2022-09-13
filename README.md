# python-setup
how to setup python playwright project in your MacOS, but you can use to start a general purpose python project as well.

# prequisite 
You should already have python3 install in your computer, if not, go to [python.org](https://www.python.org/) to learn more.

# 1. Create your project folder
```commandline
mkdir playwright-demo
cd playwright-demo
pwd
```

# 2. install virtualenv. Learn more [here](https://learnpython.com/blog/how-to-use-virtualenv-python/)
```commandline
# install or upgrade your pip version
pip install --upgrade pip
# check your version
pip --version
# install virtualenv library
pip install virtualenv
```

# 3. create a virtualenv within your project
```commandline
# go to your playwright-demo folder and create a virtualenv venv folder
python3 -m venv venv
# to activate your virtualenv
source venv/bin/activate
# to check your virtualenv is activated, whereis python will show you that you will be using python inside your venv folder
whereis python
```

# 4. install libraries to your virtualenv
```commandline
pip install pytest-playwright
pip install pytest-xdist
pip install pyyaml
```

# 5. install playwright browser
```commandline
playwright install
```

# 6. test out playwright 
go to [Add Example Test section] ([https://playwright.dev/python/docs/intro](https://playwright.dev/python/docs/intro#add-example-test))
```commandline
# run the playwright script
pytest
```

