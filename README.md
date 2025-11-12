# <img src="https://anima-kit.github.io/ai-notebooks/assets/pytorch.svg" alt="PyTorch" style="width: 32px; height: 32px; vertical-align: middle;"> <img src="https://anima-kit.github.io/ai-notebooks/assets/scikitlearn.svg" alt="scikit-learn" style="width: 32px; height: 32px; vertical-align: middle;"> <img src="https://anima-kit.github.io/ai-notebooks/assets/jupyter.svg" alt="Jupyter" style="width: 32px; height: 32px; vertical-align: middle;"> AI Jupyter Notebooks

![image](https://anima-kit.github.io/ai-notebooks/assets/ai-notebooks.png)

## 🔖 About This Project 

> TL;DR
Learn the basics of AI on your local machine to solve real-world problems with step-by-step guides through interactive notebooks 🤖.

This repo consists of a series of [Jupyter][jupyter] notebooks explaining how to solve problems through using various methods of AI. We use frameworks like [Pytorch][pytorch] and [scikit-learn][scikit-learn] to train and evaluate AI models on real data obtained from various sources. We also learn how to use libraries like [Docling][docling] to parse through data and extract crucial information. 

This project is part of my broader goal to create tutorials and resources for understanding and using AI on local machines 💻. For other in depth tutorials pertaining to building agents and the local tool servers to power them, [check it out here][tutorials].

Now, let's get building!

<a id="getting-started"></a>

## 🏁 Getting Started 

1.  Clone the repo, head there, then create a Python environment:

    ```bash
    git clone https://github.com/anima-kit/ai-notebooks.git
    cd ai-notebooks
    uv venv venv
    ``` 

    <a id="gs-activate"></a>

1.  Activate the Python environment:

    ```bash
    venv/Scripts/activate
    ```

1. Install the necessary Python libraries:

    ```bash
    uv pip install torch torchvision --index-url https://download.pytorch.org/whl/cu126
    uv pip install -r requirements.txt
    ```

1. Setup Kaggle account and API key:

    > These notebooks utilize various Kaggle datasets. To download them, you'll need a *free* Kaggle account and API key.

    1.  Go to your [Kaggle account settings](https://www.kaggle.com/settings). Be sure to sign in if you haven't already done so. 
    2.  Scroll down until you see the API settings.
    3.  Click 'Create New Token' and save the `kaggle.json` file in the proper place:
        
        - For Windows: `C:\Users\{username}\.kaggle\kaggle.json`
        - For Linux: `/home/{username}/.kaggle/kaggle.json`
        - For Mac: `/Users/{username}/.kaggle/kaggle.json`

        where `{username}` is your system's user account name.

Now you can run any of the Jupyter notebooks included in the repo.

## 📝 Example Use Cases 

These tutorials are dividing into three main aspects of AI: Machine Learning (ML), Deep Learning (DL), and Reinforcement Learning (RL) and will be released periodically.

### ML

The first tutorials will be a brief introduction to [Supervised Learning][supervised-learning] (SL) as well as deep dives into the one of the simplest SL algorithms - linear regression. We use a [Kaggle][kaggle] dataset to train and evaluate a model to predict the total energy consumed given various features, and we learn techniques for improving our model which we can carry over to other learning methods. 

### DL

We start the DL tutorials with a dive into data extraction with [Docling][docling] and the [NuExtract][nuextract] model. We learn how to use Docling's document extraction module to get key information from unstructured formats like PDFs and images. 


## 📚 Next Steps & Learning Resources 

This project is part of a series on learning and using AI. For a deeper dive, [check out my tutorials][tutorials]. Topics include:

- Setting up local servers to power AI agents
- Example agent workflows (simple chatbots to specialized agents)
- Implementing complex RAG techniques
- Discussing various aspects of AI beyond agents (like these notebooks)

Want to learn AI? [Visit my portfolio][animakit] to explore more tutorials and projects!

## ⚙️ Tech 

- [Docling][docling]: For structured data extraction
- [Jupyter][jupyter]: For interactive notebooks
- [Kaggle][kaggle]: For obtaining various datasets
- [NuExtract][nuextract]: For structured data extraction
- [Pytorch][pytorch]: For building and evaluating AI models
- [scikit-learn][scikit-learn]: For building and evaluating AI models

## 🔗 Contributing 

This repo is a work in progress. If you'd like to suggest or add improvements, fix bugs or typos etc., feel free to contribute. Check out the [contributing guidelines][contributing] to get started.


[animakit]: http://anima-kit.github.io/
[contributing]: CONTRIBUTING.md
[docling]: https://www.docling.ai/
[jupyter]: https://jupyter.org/
[kaggle]: https://www.kaggle.com/
[nuextract]: https://huggingface.co/numind/NuExtract-2.0-2B
[pytorch]: https://pytorch.org/
[scikit-learn]: https://scikit-learn.org/stable/
[supervised-learning]: https://en.wikipedia.org/wiki/Supervised_learning
[tutorials]: https://anima-kit.github.io/tutorials/