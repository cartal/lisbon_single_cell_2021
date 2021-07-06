# Lisbon single cell workshop 2021

This is a repository for the notebooks used in the Single Cell workshop for the Lisbon Summer School 2021. You can also see/use these notebooks in [Google Colab](https://towardsdatascience.com/getting-started-with-google-colab-f2fff97f594c). 

To be able to run this in Colab, you will need to do the following: 

- **Open a Google account**: If you have a personal Gmail account you are good to go. Otherwise go [here](https://support.google.com/accounts/answer/27441?hl=en) and register for one. If you don't want to use your pesonal account, you can register using your university account as well. 

- **Set up GDrive**: Each Google Account comes with 15 GiB of storage free to use. You can save your data there. 

- **Get Data**: You can download the data from the www.heartcellatlas.org website. For the batch correction excercise you will need the Heart Immune Cells, and for the label transfer you will need the heart fibroblast. 

For the transfer label example using `scNym` we can either train the model on the whole heart cell atlas dataset, but this may take a while even with GPUs! To speed up things, you can save the heart model (`models/heart_scnym`) in your GDrive so it can be used to annotate the dummy dataset. 

### Correcting batches for single cell data (scRNA-Seq)

To this end, we will use [scvi-tools](https://scvi-tools.org). You can install the suite in your local machine (Linux/MacOS) with `pip install scvi-tools`. However, as with many deep learning workflows, access to a GPU will dramatically speed up things. 

You can access the notebook [here](https://colab.research.google.com/drive/1xBd2hVl6o0oAm-Qrf_E9XcnAYPDrqPG7?usp=sharing) in Colab to run the example to batch-correct cardiac immune cells. Make a copy of it and save it in your own `GDrive`.

To use it you will need to follow these steps: 

- First to download the scRNA-Seq raw counts for the cardiac immune cells directly from the [Heart Cell Atlas](https://www.heartcellatlas.org/#Visualisations) portal.
- In your `GDrive` home directory create the folders needed for the following path: `/INBOX/lisbon_2021/raw_data/`. You can also create your own path.  
- Upload your `anndata` object inside `/INBOX/lisbon_2021/raw_data/`.  
- Update the path to the object in the CoLab notebook. 

You are good to go!

### Accessing files from CoLab

To be able to access datasets from Colab, we need to store them 

