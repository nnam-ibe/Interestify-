# Interestify
An application that uses Twitter data to determine user interest in a particular topic.

## Getting started

### Setting up Backend
Install pipenv
```bash
brew install pipenv
```
Create virtual environment
```bash
pipenv --three
```
Install project dependencies
```bash
pipenv install --dev
```
Activate virtual environment
```bash
pipenv shell
```
Download sample tweets from NLTK
```python
# Start an interative python session
python3
# import the nltk
import nltk
# Download the sample tweets from the NLTK package
nltk.download('twitter_samples')
nltk.download('punkt')
nltk.download('wordnet')
nltk.download('averaged_perceptron_tagger')
nltk.download('stopwords')
# Use exit() or Ctrl-D to exit 
```
#### Adding/Updating python packages
When installing new packages, use `pipenv` when install new packages
```bash
# e.g. sample package called colors
pipenv install colors --dev
```
### Setting up Frontend
Install dependencies
```bash
cd client/
yarn
```
#### Serve from flask
To server the frontend from the server, we first need to build the app.
```bash
yarn build
```
**Note**: This is not how you would work on the frontend.

#### Working on the frontend
To work on the frontend use the react development server, to avoid having to build after every change. See `client/README.md` for more info
```bash
yarn start
```
 
#### Adding/Updating JS packages
New packages should be installed with `yarn` which updated the `package.json` file and the lockfile `yarn.lock`
```bash
# e.g. installing the package colors
cd client/
yarn add colors
```
