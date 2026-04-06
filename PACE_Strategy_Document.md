# PACE Strategy Document: TikTok Classification Project

## 1. Plan Phase (P - Plan)
**Objective:** Understand the dataset and define the data cleaning strategy.

* **Business Problem:** Our goal is to automatically classify TikTok videos as either a 'claim' or an 'opinion'.
* **Key Question:** Which user engagement behaviors (likes, views, shares) are the most effective indicators of a "claim" video?
* **Data Source:** `tiktok_dataset.csv`

## 2. Analyze Phase (A - Analyze)
**Objective:** Discover structural issues and patterns within the data.

* **Data Cleaning:** Identify missing values (NaN) and manage null entries in critical columns such as `video_view_count`.
* **Exploratory Data Analysis (EDA):** Detect outliers. (e.g., Do videos with millions of views skew the overall distribution?)
* **Visualization:** Examine the correlation between view counts and like counts.

## 3. Construct Phase (C - Construct)
**Objective:** Engineer new, meaningful features to power the model.

* **Feature Engineering:** * `likes_per_view`: Ratio of likes to views.
    * `comments_per_view`: Ratio of comments to views.
* **Data Transformation:** Prepare categorical variables (such as `verified_status` and `author_ban_status`) for machine learning.

## 4. Execute Phase (E - Execute)
**Objective:** Share insights and propose next steps.

* **Reporting:** Summarize all findings in the `Executive_Summary.md` file.
* **Model Recommendation:** Propose using Logistic Regression or Random Forest models for the upcoming classification task.
The visualization confirmed a strong correlation between claim_status and video_view_count.

Feature engineering successfully created engagement rate variables.