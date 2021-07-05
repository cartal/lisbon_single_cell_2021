# Lisbon single cell workshop 2021

This is a repository for the notebooks used in the Single Cell workshop for the Lisbon Summer School 2021. You can also see/use these notebooks in [Google Colab](https://towardsdatascience.com/getting-started-with-google-colab-f2fff97f594c). 

To be able to run this in Colab, you will need to do the following: 

- **Open a Google account**: If you have a personal Gmail account you are good to go. Otherwise go [here](https://support.google.com/accounts/answer/27441?hl=en) and register for one. If you don't want to use your pesonal account, you can register using your university account as well. 
- **Set up GDrive**: Each Google Account comes with 15 GiB of storage free to use. You can save your data there. 
- **Get Data**: You can download the data from the www.heartcellatlas.org website. For the batch correction excercise you will need the Heart Immune Cells, and for the label transfer you will need the heart fibroblast. 

For the transfer label example using `scNym` we can either train the model on the whole heart cell atlas dataset, but this may take a while even with GPUs! To speed up things, you can save the heart model (`models/heart_scnym`) in your GDrive so it can be used to annotate the dummy dataset. 

