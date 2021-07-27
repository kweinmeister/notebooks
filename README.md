**This is not an official Google product.**

# Notebooks

* [Causal Inference with Vertex AI AutoML Forecasting](#causal-inference-with-vertex-ai-automl-forecasting)
* [Medical Imaging notebooks using Vertex AI](#medical-imaging-notebooks-using-vertex-ai)
* [Understand how your TensorFlow model is making predictions](#understand-how-your-tensorflow-model-is-making-predictions)
* [20 Newsgroups data import script for Google Cloud AutoML Natural Language](#20-newsgroups-data-import-script-for-google-cloud-automl-natural-language)
* [How to use the Google Cloud Natural Language API](#how-to-use-the-google-cloud-natural-language-api)

## Causal Inference with Vertex AI AutoML Forecasting

This [notebook](causal_inference_with_vertex_ai_automl_forecasting.ipynb) introduces the concept of causal inference. It shows how to estimate the effect of an intervention using the [tfcausalimpact](https://github.com/WillianFuks/tfcausalimpact) library and with [Vertex AI AutoML Forecasting](https://cloud.google.com/vertex-ai/docs/training/automl-console#forecasting).

## Medical Imaging notebooks using Vertex AI

The [pipeline notebook](medical_imaging_pipeline.ipynb) should be run first. It will pre-process DICOM medical images in the dataset (which needs to be downloaded prior to running). Then, it will create an AutoML model, and deploy it to an endpoint. It demonstrates how to build a pipeline using standard and custom components.

The [custom training notebook](medical_imaging_custom_training.ipynb) can be run afterward. It shows how to train a TensorFlow model using the same managed dataset.

## Understand how your TensorFlow model is making predictions

This [notebook](tensorflow-shap-college-debt.ipynb) demonstrates how to build a model using  [tf.keras](https://www.tensorflow.org/api_docs/python/tf/keras)  and then analyze its feature importances using the [SHAP](https://github.com/slundberg/shap) library.

The model predicts the expected debt-to-earnings ratio of a university's graduates. It uses data from the US Department of Education's [College Scorecard](https://collegescorecard.ed.gov/data/).

More details about the model can be found in the [blog post](https://medium.com/@kweinmeister/understand-how-your-tensorflow-model-is-making-predictions-d0b3c7e88500).

You can run the model [live in Colab with zero setup here](https://colab.research.google.com/github/kweinmeister/notebooks/blob/master/tensorflow-shap-college-debt.ipynb).

To run it locally, make sure you have Jupyter installed (`pip install jupyter`).

I've included the model code as a Jupyter notebook (`tensorflow-shap-college-debt.ipynb`). From the root directory run `jupyter notebook` to start your notebook. Then navigate to `localhost:8888` and click on `tensorflow-shap-college-debt.ipynb`.

## 20 Newsgroups data import script for Google Cloud AutoML Natural Language

This [notebook](20_newsgroups_automl.ipynb) downloads the [20 newsgroups dataset](https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html) using scikit-learn. This dataset contains about 18000 posts from 20 newsgroups, and is useful for text classification. The script transforms the data into a pandas dataframe and finally into a CSV file readable by [Google Cloud AutoML Natural Language](https://cloud.google.com/natural-language/automl).

## How to use the Google Cloud Natural Language API

This [notebook](google_cloud_natural_language_api.ipynb) demonstrates how to perform natural language tasks such as entity extraction, text classification, sentiment analysis, and syntax analysis using the [Google Cloud Natural Language API](https://cloud.google.com/natural-language/docs).
