# Spam Detection: A Little More Than Just Classifying Emails 📧

A machine learning project where I explored how to distinguish spam from normal emails. But the interesting part wasn't just training a model — it was understanding the data and figuring out what actually makes a difference.

### What I did

- Explored the Enron-Spam dataset, its class distribution, and duplicate emails with conflicting labels.
- Investigated potential features such as URLs, emojis, uppercase letters, HTML content, and email length.
- Used TF-IDF (unigrams and bigrams) alongside numerical features.
- Compared Naive Bayes, Logistic Regression, and LinearSVC.
- Used group-aware splitting and cross-validation to prevent duplicate emails from leaking across datasets.
- Tuned LinearSVC and performed an ablation study to evaluate the contribution of additional features.

### Results & Takeaways

The final LinearSVC model achieved approximately **0.99 F1-score** on the held-out test set.

Interestingly, adding more features barely improved performance. TF-IDF was already doing most of the work.

A few things I learned:

- High scores don't automatically mean good experiments.
- Data quality and duplicate samples matter.
- Feature engineering should be tested, not just assumed to be useful.
- Understanding model errors can be as valuable as improving performance.

### What's next?

I'd like to test the model on an entirely different email dataset to see how well it generalizes beyond the Enron environment.

Because doing well on one dataset is nice, but let's see how it behaves in the real world. :)

---

*Built with Python, Pandas, NumPy, NLTK, Matplotlib, Seaborn, and Scikit-learn.*



`Made with love by Atena Rahimi ♡`


