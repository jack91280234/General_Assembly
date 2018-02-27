# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 4: Web Scraping & Classification

### Description

This project helps you practice webscraping, NLP and classification models.

### Scenario

You're fresh out of your Data Science bootcamp and looking to break through in the world of freelance data journalism. Nate Silver and co. at FiveThirtyEight have agreed to hear your pitch for a story in two weeks!

Your piece is going to be on how to create a Reddit post that will get the most engagement from Reddit users. Because this is FiveThirtyEight, you're going to have to get data and analyze it in order to make a compelling narrative.

#### Project Summary

In this project, we will practice two major skills. Collecting data by scraping a website and then building a binary predictor.

There are two components to starting a data science problem: the problem statement, and acquiring the data.

For this article, your problem statement will be: _What characteristics of a post on Reddit are most predictive of the overall interaction on a thread (as measured by number of comments)?_

Your method for acquiring the data will be scraping the 'hot' threads as listed on the [Reddit homepage](https://www.reddit.com/). You'll acquire _AT LEAST FOUR_ pieces of information about each thread:
1. The title of the thread
2. The subreddit that the thread corresponds to
3. The length of time it has been up on Reddit
4. The number of comments on the thread

Once you've got the data, you will build a classification model that, using Natural Language Processing and any other relevant features, predicts whether or not a given Reddit post will have above or below the _median_ number of comments.

**BONUS PROBLEMS**
1. Scrape the full text of the threads using Selenium.
2. Write the actual article that you're pitching and turn it into a blog post that you host on your personal blog.

---

### Requirements

- Scrape and prepare your data using BeautifulSoup.
    - We have provided a sample dataset for you.  If you cannot scrape, you can use this data for your modeling, but one of the goals of this project is to practice scraping.  Use this dataset as a last resort!
- **Create and compare two models**. One of these must be a random forest, however the other can be a classifier of your choosing: logistic regression, KNN, SVM, etc.
- A Jupyter Notebook with your analysis for a peer audience of data scientists.
- An executive summary of the results you found.
- A 4 minute presentation outlining your process and findings for a semi-technical audience. The reason we say 'semi-technical' is that FiveThirtyEight wants to see how you plan to explain your findings in your article, and their audience is likely readers who are familiar with and interested in data / statistics, but are not experts. This means that if you'd like to talk about your model works you can, but explain what exactly your model does at a high-level.

 **Pro Tip:** You can find a good example executive summary [here](https://www.proposify.biz/blog/executive-summary).

 **Pro Tip 2:** When building your webscraper, use the `sleep` function to make time in between your individual requests.  Check reddit's API documentation to see how many calls they allow.  

 **Pro Tip 3:** Build your scraper, and rigorously test it on a few pages to make sure it works before setting it loose on all of Reddit.

 **Pro tip 4:** Scrape early, scrape often. Unlike earlier projects, you're collecting your own data, and you won't be able to even start modeling until you've collected all of this.

**Pro tip 5:** Save your results to a .csv or .txt file whenever you scrape. If you just keep your results in memory, if you computer crashes or shuts off, or you accidentally close your Jupyter notebook, you'll lose your data.

---

### Necessary Deliverables / Submission

- Code and executive summary must be in a clearly commented Jupyter Notebook.
- You must submit your slide deck.
- Materials must be submitted by 9 a.m. Friday, January 26 EST.

---

### Dataset

1. We'll be utilizing a dataset derived from live web data: [Reddit.com](https://www.reddit.com/)

2. To get the data, we will use the requests library (or urllib, or chromedriver) and BeautifulSoup to scrape the webpage.

---


### Additional Resources
- [Advice on How to Write for a Non-Technical Audience](http://programmers.stackexchange.com/questions/11523/explaining-technical-things-to-non-technical-people)
- [Documentation for BeautifulSoup can be found here](http://www.crummy.com/software/BeautifulSoup/).

---

### Project Feedback + Evaluation

Data science is a field in which we apply data to solve real-world problems. Therefore, projects and presentations are means by which we can assess your ability to solve real-world problems in a data-driven manner.

When evaluating projects, there are four areas on which your instructors focus.
1. **Project Requirements: Did you meet all project requirements?** In answering this question, your instructors want to assess how well you met the project requirements as established. These will generally be laid out in the project readme.

2. **Audience: Is your presentation appropriate for the stakeholder?** In answering this question, your instructors want to assess how well you present your results to stakeholders. For example:
  - Did you frame the problem appropriately for the audience?
  - Did you use the appropriate level of technical language for your audience?
  - Did you effectively use your time, or did you encounter an issue such as going significantly beyond or under the allotted time or rushing to conclude the presentation in the allotted time?
  - Did you present effectively, or were there things that detract from the overall presentation such as not speaking loudly enough for the audience or repeating oneself?

3. **Methods: Are your methods appropriate for solving the problem?** In answering this question, your instructors want to assess how well you have applied data science methodology to the problem at hand. For example:
  - Did you make well-reasoned modeling choices, or is there clear evidence that the model is inadequate or improper?
  - Are you able to clearly defend your methodological decisions and results?
  - Did you generalize your results properly, or were your conclusions/inferences improper or fallacious?

4. **Value: Have you provided value to the stakeholder through clear, data-driven recommendations?** In answering this question, your instructors want to assess the value you provide to the stakeholder as a data scientist. For example:
  - Did you answer the problem posed to you?
  - Did you make your recommendations clear, or were the recommendations unclear?
  - Were your recommendations data-driven and based on the results of your work?

You will earn a score for each of the four areas mentioned above.
1. Data Collection / Cleaning: You may earn a score between 0 and 2.  A score of 0 means your data is not appropriately cleaned.  A score of 1 means that you were not able to scrape your own data, but your data munging was adequate.  If you do not scrape your data, the maximum you can receive is 1.  A score of 2 means you appropriately scraped and cleaned your data.
2. Audience: You may earn a score between 0 and 2. A score of 0 indicates that your presentation is inappropriate for the stakeholder. A score of 1 indicates that at least part of your presentation should be non-trivially reworked to be more appropriate for the stakeholder. A score of 2 indicates that there are few to no areas of your presentation that should be reworked.
3. Methods: You may earn a score between 0 and 2. A score of 0 indicates that your methods are inappropriate. A score of 1 indicates that your methods are somewhat inappropriate, that justification for methodological decisions is lacking, and/or that your conclusions do not follow from the methods. A score of 2 indicates that your methods are appropriate, justification is sufficient/strong, and your conclusions follow well from the methods.
4. Value: You may earn a score between 0 and 2. A score of 0 indicates that you provide little to no value to the stakeholder. A score of 1 indicates that the value you provide to the stakeholder is substantially less than expected by not answering the problem, not providing clear recommendations to the stakeholder, and/or providing recommendations that were not data-driven. A score of 2 indicates that the value you provide to the stakeholder is on par with the expectation of providing clear, data-driven recommendations that directly answer the problem posed.
