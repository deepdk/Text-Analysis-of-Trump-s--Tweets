# Text Analysis of Trump's Tweets

When Trump wished the Olympic team good luck, he was tweeting from an iPhone. When he insulted a rival, he was usually tweeting from an Android. Is this an artifact showing which tweets are Trump’s own and which are by some handler in the 2016 campaign?

Others have explored Trump’s timeline and noticed this tends to hold up. And Trump himself did indeed tweet from a Samsung Galaxy until March 2017. But how could we examine it quantitatively?

## 🔎Background

![image](https://user-images.githubusercontent.com/31981663/201830361-efe6fc01-69a2-4b37-b7c3-326460cc0ba8.png)

Dataset is from The [Trump Twitter Archive](http://www.trumptwitterarchive.com/) by Brendan Brown, which contains all 35,000+ tweets from the @realDonaldTrump Twitter account from 2009 (the year Trump sent his first tweet) through 2018.

## 📊EDA

### Time of Tweeting

![image](https://user-images.githubusercontent.com/31981663/201830695-2f0a56ec-54af-4321-a122-7c9d668b5d4e.png)

📌 **We can certainly spot the difference here. Most tweets from the Android are in the early morning or later in the evening, while tweets from the iPhone occur more often in the afternoon.**

### Quote Tweets

![image](https://user-images.githubusercontent.com/31981663/201830862-395add9d-cfdd-498e-9e80-d0686d56ad58.png)

📌 **Almost all the quote tweets are posted from the Android.**

### Tweets containing links and pictures

![image](https://user-images.githubusercontent.com/31981663/201830965-360cf103-7ed5-4914-a069-04875c131674.png)

📌 **It turns out that tweets from the iPhone were way more likely to contain either a picture or a link. This also makes sense with our narrative: iPhone (presumably run by the campaign) tends to write “announcement” tweets about events**

### Common Words : Android Vs iPhone

![image](https://user-images.githubusercontent.com/31981663/201831612-c32c4986-140a-44e7-ab63-1f7d8430d099.png)

📌 ** Calculated the log odds ratio of each word, we'll plot the 15 words with the greatest log odds ratio for the Android and the iPhone.
With the way we've set up the log odds ratio, positive values are assigned to words from the Android, and negative values are assigned to the iPhone.**

### Frequency of Each Word

![image](https://user-images.githubusercontent.com/31981663/201831817-265c728b-f9cc-4cca-ae8a-3111a4899d79.png)

📌 **We can see the difference of sentiments**

## 🔎Conclusion

There's a difference in style and sentiment between Trump's tweets from the Android and the iPhone. We know Trump used the Android until March 2017, but who was tweeting from the iPhone on Trump's behalf? It's fascinationg to read a New Yorker article about Tony Schwartz, Trump’s ghostwriter for The Art of the Deal. Of particular interest was how Schwartz imitated Trump’s voice and philosophy:

In his journal, Schwartz describes the process of trying to make Trump’s voice palatable in the book. It was kind of “a trick,” he writes, to mimic Trump’s blunt, staccato, no-apologies delivery while making him seem almost boyishly appealing…. Looking back at the text now, Schwartz says, “I created a character far more winning than Trump is.”

A lot has been written about Trump’s mental state. But it's rather get inside the head of the anonymous staffer whose job is to imitate Trump’s unique cadence (“Very sad!”) or put a positive spin on it, to millions of his followers. Are they a true believer, or just a cog in a political machine, mixing whatever mainstream appeal they can into the @realDonaldTrump concoction? Like Tony Schwartz, will they one day regret their involvement?



