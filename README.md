# Hate Raids on Twitch
This is the R code behind my paper, "Couldn’t Protect You: The Cost of (Hate) Raids on Smaller Streamers," which was completed in collaboration with Dr. Rachel Kowert.

## Order of Operation
1. Data Collection
2. Data Visualization
3. Data Analyses
4. Hate Raids


### Data Notes
The CSV files in `data/` follow the X Developer Policy on content redistribution: they carry tweet IDs, conversation and quoted-tweet IDs, timestamps, language, public engagement counts, and derived scores only. No tweet text, usernames, user IDs, or profile fields are included. In `pre_release.csv` and `post_release.csv`, `analysed` marks the tweets the analysis scores (no game-title terms, conversation starters only), and `sent_value`, the ten NRC Word-Emotion Association Lexicon counts, and `emo_score` (positive minus negative) are the scores `full_script.R` computes for them. To rerun the text steps, retrieve ("hydrate") the tweets from the X API with your own credentials; tweets deleted or made private since collection will not be returned.

## License

The code is released under the MIT License (see `LICENSE`). Use of the tweet IDs to retrieve content from X is governed by the X Terms of Service, Privacy Policy, Developer Agreement, and Developer Policy.

### Finding Preview
Below are the figures used in the paper.

#### Figure A1

*Tweets Announcing the Release of New Twitch Tags*

![Figure 1](https://raw.githubusercontent.com/apleith/hate-raids/main/images/fig1.png)

#### Figure A2

*Number of “Twitch Raid” Tweets per Day*

![Figure 2](https://raw.githubusercontent.com/apleith/hate-raids/main/images/fig2.png)

#### Figure A3

*Comparison of Emotional Score for Pre-Release and Post-Release Tweets*

![Figure 3](https://raw.githubusercontent.com/apleith/hate-raids/main/images/fig3.png)

#### Figure A4

*Comparison of Engagement Score for Pre-Release and Post-Release Tweets*

![Figure 4](https://raw.githubusercontent.com/apleith/hate-raids/main/images/fig4.png)

#### Figure A5

*Frequency of Hate Raids Tweets from May 26 - November 25, 2021*

![Figure 5](https://raw.githubusercontent.com/apleith/hate-raids/main/images/fig5.png)
