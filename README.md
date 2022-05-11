# Project title (2022 Spring DM)
Wordle 1

* Team members: Anjnesh Sharma, Yunpeng Guo, Renjie Xu
* Project paper: https://github.com/class-data-mining-master/2022-spring-dm-project-2022-spring-team01-wellerman/blob/2d7de6b5469fcd63304463e707555ab4e045ee38/Project%20paper.pdf

## Description

Wordle is an online word game that looks a lot like classic code-breaking, color-coded board games like Mastermind, but it's even easier to play. Every day, a new, mysterious five-letter word must be guessed, which must be done by typing five-letter words into Wordle's 30 tile grid. Usually a normal user has to take 3.9 attempts to guess the correct word of the day, and our goal is to develop a system that can predict the day’s word in the first attempt, by analysing the results shared by people on Twitter. 

The Wordle source code contains 2,315 days of answers that are all common 5-letter English words and 10,657 other valid, less-common 5-letter English words. We combine these to form a set of 12,972 possible words/answers. We then simulate playing 3000 Wordle games for each of these possible words, guessing based on the frequency of the word in the English language and the feedback received. We take three measures to evaluate the observed distribution of squares on Twitter according to our valid words. We then generate our guess by taking the word with the best average rank across these three measures

directories of this repository:
|-- Readme.md                             // help file
|-- requirement.txt                       // additional required python package
|-- wordle16.ipynb                        // Performs the word prediction
|-- word simulation.ipynb                 // Performs word simulations and saves results as pickle files
|-- ScrapeTweets.ipynb                    // Pulls tweets from Twitter
...

## Running the code

First run ScrapeTweets.ipynb to pull player tweets for the day

We have uploaded the pickle files for word simulations so running that won't be necessary.

Run wordle16 to predict the day's word.

## Prerequisites

Python packages required for the scraping part: tweepy, pytz, re
Python packages required for wordle16: pickle
Python packages required for word simulation: ray, pickle
Other requirements: Since the tweepy is the twitter's official package for scraping data from twitter, a twitter developer account is needed and due to the license it will not be provided in this repository.

## Authors
Anjnesh Sharma: ans458@pitt.edu
Yunpeng Guo: yug64@pitt.edu
Renjie Xu: rj.xu@pitt.edu

## Acknowledgments

We would like to expresss our gratitude to Dr. Yuru Lin for her teaching of the data mining processes that inspired us to dig knowledge from the user tweets data and apply them to solve the world puzzle. Also, we would like to thank twitter for providing powerful api to acquire the data we need in a much easier way.


## License

[MIT](https://choosealicense.com/licenses/mit/)
