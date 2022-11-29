# Negative Sentiment Shift on a Chinese  Movie-rating Website

### Abstract:

Polarized sentiment plays a key role in group polarization, and shifting to negativity is more commonly seen in online communities (Zollo, Novak, et. al., 2015, Del, Vivaldo, et. al., 2016, Abisheva, Garcia, et. al., 2016). Nevertheless, a negative sentiment shift could be detrimental to the online community (Cheng, Danescu-Niculescu-Mizil, & Leskovec 2014, May). When current research often links negative sentiment shifts with echo chambers and misinformation (Bessi, Petroni, et al., 2015), it’s also argued that the echo chamber may be overstated (Dubois & Blank 2018). Here, we explore the sentiment drift using over 4 million comments from a Chinese online movie-rating community that is less affected by misinformation compared to mainstream online communities. We measure the sentiment shift of the community and users of different engagement levels. Our analysis reveals that while the community doesn’t show a tendency toward negativity, users of higher engagement levels are generally more negative, considering factors like the different movies they consume. The results indicate a fitting-in process, suggesting the possible mechanism of group identity on sentiment shift ion on social media platforms.

### Data:

The whole dataset is over 800MB(over 4 million comments), making it unsuitable for storing on Github. So here a sample of 5000 movie comments is uploaded). The data used for fine-tuning BERT is also included. 

**Link to scraping program and full-size dataset**:https://github.com/csuldw/AntSpider

### Code:

**Sentiment_analysis**: `Analyze_comments.ipynb`

The sentiment-based analysis could be run locally. The code is written in python 3.8.5. and all of its dependencies can be installed by running the following in the terminal (with the `requirements_analysis.txt` file included in this repository):

```
pip install -r requirements_analysis.txt
```



**Fine-tuning BERT and getting sentiment labels**:`Fine_tune_BERT.ipynb`

The code run on Colab is written in python 3.8.5.  All of its dependencies can be installed by running the following in the terminal (with the `requirements_fine_tuning.txt` file included in this repository):

```
pip install -r requirements_fine_tuning.txt
```



Then you can download all the datasets and replace the directories specified in the code with your own directories, and run all the cell in sequence to reproduce all the results. Noting that data set contains over 4 million comments, getting labels and analyze may take over 100 hours. Future code may parallelize the computing process. 



### How to cite:

```
@software{Hongkai040,
  author       = {Hongkai Mao},
  title        = {Negative Sentiment Shift on a Chinese  Movie-rating Website},
  month        = Nov,
  year         = 2022,
  publisher    = {Github},
  journal      = {Github repository},
  howpublished = {\url{https://github.com/Hongkai040/Negative_Sentiment_Shift_in_Online_Community}},
  commit       = {}
}
```
