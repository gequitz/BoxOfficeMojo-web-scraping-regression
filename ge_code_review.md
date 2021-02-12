# Code Review: Project 2

### Name: Gabriel Equitz

[X] README.md included

[X] Slides included

[X] Code included

## Clean Code:
- Use comments and markdown cells a lot more frequently to make it clear what your code is doing and the intention of each step in your analysis! Your future self and any collaborators will thank you!
- Try not to leave draft code that's been entirely commented out or that you're no longer using in the final version of your notebooks/scripts. 
- 4-6 seconds is *probably* too long of a pause to take between every step of your scraper. You should only need 0-2 seconds.
- Really great work defining functions to scrape bomojo! A next step would be separating these out into a separate .py file and importing them in your notebook.
- Try to avoid leaving really long cell outputs in your final notebook, since they make it harder for others to review your analysis, e.g. where you print out the entirety of `mojo_dict_list`.
- I'd suggest breaking up your project across different notebooks and using pickle files to transfer data from one to the next. Having things segmented makes it easier to review and de-bug. And more importantly, right now there's no way to reproduce your analysis withour re-running the scraper. You want to make sure you have the raw data saved somewhere so your analysis and results can be reproduced without needing to re-scrape.
- Try and do things programmatically when possible. E.g. instead of writing one-off, separate lines of code for creating dummy variables for genres, you could use a for loop, for example something like:


        for g in [genre_list]:

            df[g] = df['genres'].apply(lambda x : 1 if g in x else 0)

## Good Documentation:
- Good work including a detailed readme!
- I'd suggest using the first person singular (i.e. "I" instead of "we" to make it clear that you did all this work independently!)
- Seems trivial, but I'd suggest including your slides in pdf format in your github repo, since .key files can't be previewed, and you probably want others to be able to view directly in the browser!

## Proper Data Science:
- It seems like you may have limited your scrape to only 200 movies? If that's the case, I'd definitely recommend scraping more data. More data = more opportunity for your model to pick up on patterns/signals -- 200 is a very small sample. Also, make sure you consider any sampling bias that could be introduced by selecting the first 200 in a list rather than a random sample of 200 (depends on whether/how the original list was sorted!). If there is a bias to your sample that could mean your model won't generalize well to out-of-sample data.
- It's not clear to me why you had a few different regression models created with just a single feature. If you're interested in exploring the bivariate relationships between a feature and your target, do that as part of your EDA process by creating charts or calculating the correlation between the two variables.
- Good job using LassoCV to try and evaluate different alpha levels!
- Good work separating out train, validation, and test data!
- Anytime you're getting a negative R^2, that should raise some alarm bells about your modeling process; it means your model is performing worse than a simple model that just predicts the mean for every observation would. My *guess* is that you're seeing this because your dataset is so small that your model just doesn't have enough to learn from in the training data. I'd revisit your scraping to pull a lot more data, then try feeding that through your modeling workflow!