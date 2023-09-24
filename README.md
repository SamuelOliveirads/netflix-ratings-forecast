# netflix_ratings_forecast

## Overview

This is your new Kedro project, which was generated using `Kedro 0.18.12`.

Take a look at the [Kedro documentation](https://kedro.readthedocs.io) to get started.

### Business problem

Netflix is looking to develop a predictive model to forecast movie ratings, thereby determining whether it's worthwhile to add a particular movie to their catalog.
The challenge is to construct a machine learning model that predicts the rating a movie would receive if added to the catalog.

Here is the [solution planning](docs/planning.md)

## Solution strategy
To solve the business problem I use the CRISP-DM methodology adapted for data science processes, the process steps for the solution will be as follows:

![crisp-method](/docs/crisp_ds.png)

This process guarantees the construction of quick projects that allow potential problems to be visualized at every stage, as well as implementing continuous improvement with each new cycle.

## Notebook structure
The notebooks take advantage of Kedro's structure to be modular, allowing each stage of the solution to be a single notebook, the version in the notebook's name corresponds to the project cycle where each cycle represents a potential delivery for the interested party.
> Note: To ensure that the notebook runs, it is important to install the dependencies and run the notebooks sequentially.

## Rules and guidelines

In order to get the best out of the template:

* Don't remove any lines from the `.gitignore` file we provide
* Make sure your results can be reproduced by following a [data engineering convention](https://kedro.readthedocs.io/en/stable/faq/faq.html#what-is-data-engineering-convention)
* Don't commit data to your repository
* Don't commit any credentials or your local configuration to your repository. Keep all your credentials and local configuration in `conf/local/`

## How to install dependencies

Declare any dependencies in `src/requirements.txt` for `pip` installation and `src/environment.yml` for `conda` installation.

To install them, run:

```
pip install -r src/requirements.txt
```


## How to work with Kedro and notebooks

> Note: Using `kedro jupyter` or `kedro ipython` to run your notebook provides these variables in scope: `catalog`, `context`, `pipelines` and `session`.
>
> Jupyter, JupyterLab, and IPython are already included in the project requirements by default, so once you have run `pip install -r src/requirements.txt` you will not need to take any extra steps before you use them.

### Jupyter
To use Jupyter notebooks in your Kedro project, you need to install Jupyter:

```
pip install jupyter
```

After installing Jupyter, you can start a local notebook server:

```
kedro jupyter notebook
```

### JupyterLab
To use JupyterLab, you need to install it:

```
pip install jupyterlab
```

You can also start JupyterLab:

```
kedro jupyter lab
```

### IPython
And if you want to run an IPython session:

```
kedro ipython
```

## Conclusions
- The delivery of the model represents a list of films in production with expected high customer ratings, which allows Netflix to improve its quality of service and satisfaction.
- The optimization of resources by revenue expectation helps in the allocation and choice of which films to select if budget is a limiting factor.

## Next steps
- **Deploy the model**: think about the type of deployment
- **Collect more data**: there could be more lines, the filling in of nans, especially directors could come from collection
- **Analyze more hypotheses**: we have a list of hypotheses to validate, plus along the way we've noticed more hypotheses that could be evaluated.
- **Features**: Develop features that segment the genres, directors, team and synopsis
- **Machine Learning**: Testing new models that exploit data from other formats such as neural networks, Support Vector Machines, polynomial regressions, as well as developing ensemble models that combine the different models.
- **Fine tuning**: this step was carefully skipped due to the use of linear regression, but with new models it may become a necessary step.
- **Analyze perceived noise in model errors**: especially data with divergent behavior and outliers.
- **Modularize**: reduce code repetition with the help of functions for processing steps, fine tuning and business scenarios.
- **Resource optimization**: Improve the optimization rules for business by considering a more robust optimization such as knapsack.
