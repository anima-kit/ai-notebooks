# <img src="https://anima-kit.github.io/ai-notebooks/assets/pytorch.svg" alt="PyTorch" style="width: 32px; height: 32px; vertical-align: middle;"> <img src="https://anima-kit.github.io/ai-notebooks/assets/scikitlearn.svg" alt="scikit-learn" style="width: 32px; height: 32px; vertical-align: middle;"> <img src="https://anima-kit.github.io/ai-notebooks/assets/jupyter.svg" alt="Jupyter" style="width: 32px; height: 32px; vertical-align: middle;"> AI Jupyter Notebooks

![image](https://anima-kit.github.io/ai-notebooks/assets/ai-notebooks.png)

## 🔖 About This Project 

> TL;DR
Learn the basics of AI on your local machine to solve real-world problems with step-by-step guides through interactive notebooks 🤖.

This repo consists of a series of [Jupyter][jupyter] notebooks explaining how to solve problems through using various methods of AI. We use [Pytorch][pytorch] and [scikit-learn][scikit-learn] to train and evaluate AI models on real data obtained from various sources. Each notebook is a step-by-step guide of how to solve a given problem with in-depth descriptions of the supporting math and code.

This project is part of my broader goal to create tutorials and resources for understanding and using AI on local machines 💻. For other in depth tutorials pertaining to building agents and the local tool servers to power them, [check it out here][tutorials].

Now, let's get building!

## 🏁 Getting Started 

1.  Clone the repo, head there, then create a Python environment:

    ```bash
    git clone https://github.com/anima-kit/ai-notebooks.git
    cd ai-notebooks
    python -m venv venv
    ``` 

    <a id="gs-activate"></a>

1.  Activate the Python environment:

    ```bash
    venv/Scripts/activate
    ```

1. Install the necessary Python libraries:

    ```bash
    pip install -r requirements.txt
    ```

1.  Now you can run any of the Jupyter notebooks included in the repo.

## 📝 Example Use Cases 

I plan on dividing tutorials into three main aspects of AI: Machine Learning (ML), Deep Learning (DL), and Reinforcement Learning (RL). Tutorials will be released periodically starting with the basics of ML which can be found in the `./00-ML` folder.

The first tutorials will be a brief introduction to [Supervised Learning][supervised-learning] (SL) as well as deep dives into the one of the simplest SL algorithms - linear regression. We use a [Kaggle][kaggle] dataset to train and evaluate a model to predict the total energy consumed given various features, and we learn techniques for improving our model which we can carry over to other learning methods. 

## 📚 Next Steps & Learning Resources 

This project is part of a series on learning and using AI. For a deeper dive, [check out my tutorials][tutorials]. Topics include:

- Setting up local servers to power AI agents
- Example agent workflows (simple chatbots to specialized agents)
- Implementing complex RAG techniques
- Discussing various aspects of AI beyond agents (like these notebooks)

Want to learn AI? [Visit my portfolio][animakit] to explore more tutorials and projects!

## 🏯 Project Structure

```
├── 00-ML/                          # Folder containing all ML notebooks
│   └── 00-regression/              # Folder containing all regression notebooks
│       └── 00-basics.ipynb         # First tutorial for regression basics
│       └── 01-preprocessing.ipynb  # First tutorial for regression basics
├── requirements.txt                # Required Python libraries for main app
```

## ⚙️ Tech 

- [Jupyter][jupyter]: For interactive notebooks
- [Pytorch][pytorch]: For building and evaluating AI models
- [scikit-learn][scikit-learn]: For building and evaluating AI models
- [Kaggle][kaggle]: For obtaining various datasets

## 🔗 Contributing 

This repo is a work in progress. If you'd like to suggest or add improvements, fix bugs or typos etc., feel free to contribute. Check out the [contributing guidelines][contributing] to get started.


[animakit]: http://anima-kit.github.io/
[contributing]: CONTRIBUTING.md
[jupyter]: https://jupyter.org/
[kaggle]: https://www.kaggle.com/
[pytorch]: https://pytorch.org/
[scikit-learn]: https://scikit-learn.org/stable/
[supervised-learning]: https://en.wikipedia.org/wiki/Supervised_learning
[tutorials]: https://anima-kit.github.io/tutorials/