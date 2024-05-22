# geeksessions-streamlit, May 22, 2024
streamlit dashboard kickstarter

* Minimalistic way how to create `streamlit` interactive dashboard using exemplary ML Iris dataset. 
* With 130 lines of code, you train model, visualize results, and create interactive environment for the user to look into your KMeans clustering.

## Before running the app
* to investigate how the codes work, play with the jupyter NB
* Btw. Colab has free GPU support, if you ever need it for ML testing.
* This can be done using the links below, no python needed.

|   | Run | Run | View |
| - | --- | --- | ---- |
| Iris dataset | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Py-ualg/geeksessions-streamlit/blob/main/iris_processing.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Py-ualg/geeksessions-streamlit/HEAD?labpath=iris_processing.ipynb) | [![View the notebook](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/Py-ualg/geeksessions-streamlit/blob/main/iris_processing.ipynb?flush_cache=true)

## To run the app
1. Clone the repository

## Running locally
* `pip install -r requirements.txt`
* `streamlit run app.py`
* In the upper right hand corner is option to deploy the app.

## No python
1. You can still deploy and edit with codespaces without much testing though.
2. Go to [streamlit](https://streamlit.io)
3. Sign in with GH, gmail or other
    * If you want to run dashboard from your organization, follow instructions [here](https://docs.github.com/en/organizations/managing-oauth-access-to-your-organizations-data/about-oauth-app-access-restrictions)
4. Create app
    * repo: Py-ualg/geeksessions-streamlit
    * branch: main
    * Main file-path: app.py
    * app URL: UP-TO-YOU.
5. You should have the app functional and running

## Two ways to continue
### Expand the dashboard capabilities individually
1. For each input, in addition to classification, show also the probabilities of classes
    * KMeans are not good for that, perhaps try [XBoost classifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html#sklearn.ensemble.GradientBoostingClassifier).
2. `Model` tab: How to visualize the 4D data:
    * pairplot (seaborn library)
    * 3D + color hue?
    * Confusion matrix (for train and test data), [docs](https://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html#confusion-matrix).
3. `Prediction` tab: Visualize input values against testing data using the plotClusters function

### Group work: Given that not all must be interested in streamlit
1. Let's make interactive dashboard which is useful for GeekSessions community
2. List of active tech people in Algarve
3. Events
4. Contacts and calendar
5. Skills for collaborating

#### We need
* Database (tables in pandas for simplicity)
* visualization (maps, calendar, links)
* search

