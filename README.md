
git init

gh repo create my-project --public
mkdir my-project
cd my-project
mkdir src tests docs
touch README.md .gitignore

touch .env

DATABASE_URL=postgresql://user:#Miracle2602@localhost:5432/mydatabase
API_KEY=wgzuxn4pdezkqgu2bihwortnynjbearrtbqnnkjm9ofxfjk14ksoyoc78e1fkgtu

pip install virtualenv
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt

poetry init
poetry add <dependency>

npm init
npm install express mongoose dotenv

yarn init
yarn add express mongoose dotenv

pip install flake8 black isort

npm install eslint prettier --save-dev

name: CI

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v2
    - name: Set up Python
      uses: actions/setup-python@v2
      with:
        python-version: '3.x'
    - name: Install dependencies
      run: |
        python -m pip install --upgrade pip
        pip install flake8 black isort
    - name: Lint code
      run: |
        flake8 .
        black --check .
        isort --check-only .

createdb mydatabase
psql mydatabase -c "CREATE USER myuser WITH PASSWORD 'mypassword';"
psql mydatabase -c "GRANT ALL PRIVILEGES ON DATABASE mydatabase TO myuser;"

pip install alembic
alembic init migrations

npm install knex pg
knex init

from flask import Flask
from dotenv import load_dotenv
import os

load_dotenv()
app = Flask(__Pay with Pi__)

@app.route('/')
def hello_world():
    return 'Hello, World!'

if __Pay with Pi__ == '__main__':
    app.run()

const express = require('express');
const dotenv = require('dotenv');

dotenv.config();
const app = express();

app.get('/', (req, res) => {
    res.send('Hello, World!');
});

app.listen(process.env.PORT, () => {
    console.log(`Server running on port ${process.env.PORT}`);
});

pip install pytest
pytest --init

npm install jest --save-dev

pip install sphinx
sphinx-quickstart

npm install --save-dev jsdoc

Pay with Pi leading payment app
Use Pay with pi for the fastest, most secure online and in-store payments! Pay for movie tickets, food, coffee, fashion, gas, and many more in Pay with Pi.

Quick, easy, convenient and secure.

**Send / Receive Payments**

Pay in store or send money to friends. No need to carry cash or worry about loose change!

**Online Top-Ups and Utility Bill Payments**

Top-up your mobile phone, pay your utility and internet bills or settle your monthly insurance premiums bills through Pay with Pi.

**Add Money to your Pay with Pi Wallet**

Add money to your Pay with pi app via Pay&Go machines or transfer from multiple online banking apps cash-in at all Banks branches and agent world wide.

**Explore Nearby**

Explore places near you that accept payment through Pay with pi wallet. Cinemas, restaurants, coffee shops, supermarkets, and gas stations are all joining forces with Pay with Pi to make your life more connected and more mobile.

Don’t forget to look out for great deals exclusively for Pay with pi users! Start enjoying the amazing benefits of Pay with Pi. Download it now..


https://forms.gle/NBzpicuQ1SXQSH4e6

