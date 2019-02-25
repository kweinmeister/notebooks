**This is not an official Google product.**

# Notebooks

* [Understand how your TensorFlow model is making predictions]((#understand-how-your-tensorflow-model-is-making-predictions))

## Understand how your TensorFlow model is making predictions

This [notebook](tensorflow-shap-college-debt.ipynb) demonstrates how to build a model using  [tf.keras](https://www.tensorflow.org/api_docs/python/tf/keras)  and then analyze its feature importances using the [SHAP](https://github.com/slundberg/shap) library.

The model predicts the expected debt-to-earnings ratio of a university's graduates. It uses data from the US Department of Education's [College Scorecard](https://collegescorecard.ed.gov/data/).

More details about the model can be found in the [blog post](https://medium.com/@kweinmeister/understand-how-your-tensorflow-model-is-making-predictions-d0b3c7e88500).

You can run the model [live in Colab with zero setup here](https://colab.research.google.com/github/kweinmeister/notebooks/blob/master/tensorflow-shap-college-debt.ipynb).

To run it locally, make sure you have Jupyter installed (`pip install jupyter`).

I've included the model code as a Jupyter notebook (`tensorflow-shap-college-debt.ipynb`). From the root directory run `jupyter notebook` to start your notebook. Then navigate to `localhost:8888` and click on `tensorflow-shap-college-debt.ipynb`.

