---
title: "Code Meets Culture: Analyzing Hari Raya Music with YouTube API in R"
date: 2025-04-28
summary: "An R>aya Meetup and sharing session of how I used Web APIs in R"
tags: ["R Programming", "Web API", "Data Analysis"]
slug: "code-meets-culture"
draft: false
---

## TLDR;

📊 Here's what we discovered:

* YouTube API provides powerful tools to analyze video statistics and trends
* The most viewed Hari Raya music video is Omar dan Hana's song, highlighting YouTube's popularity among children
* As of April 28, 2025, "Serumpun" holds the record for most liked Hari Raya music video, while "Meriah Lain Macam" has the highest view count

---

## Introduction

_Hello, World! Selamat Hari Raya Aidilfitri to everyone celebrating!_ 🌙

I recently had the honor of presenting at the **Brunei R>aya Meetup** on April 18, 2025, hosted by the Brunei R User Group at UBD Library. The event was a fantastic opportunity to share knowledge alongside brilliant speakers:

* **Dr. Daphne Lai**: Presented on Principal Component Analysis clustering of kuih raya
* **Muaz Mahdi**: Explored eating behaviors during open houses using Markov chains

You can find more details about the event on the [Brunei R website](https://bruneir.github.io/posts/bru-25-2-raya).

In this blog post, I'll share my presentation on working with APIs in R, specifically focusing on using the YouTube API to analyze Hari Raya music trends.

## Understanding APIs 🔌

An Application Programming Interface (API) serves as a communication bridge between different software systems. To better understand this concept, let's use a restaurant analogy:

<img src="/static/what-is-api.png" alt="What is API" style="max-width:100%; height:auto;" />

APIs can be broadly categorized into two types:

1. **Data Retrieval APIs**: Used to fetch information (what we'll focus on in this post)
2. **Command/Action APIs**: Used to perform specific actions

APIs can be either:
* 🔓 **Keyless**: Free to use without authentication
* 🔑 **Key-based**: Require authentication through API keys

## Required R Packages 📦

To work with APIs in R, we'll primarily use two essential packages:

```r
# Install required packages
install.packages(c("httr", "jsonlite", "tuber"))

# Load the packages
library(httr)      # For making HTTP requests
library(jsonlite)  # For parsing JSON responses
library(tuber)     # For YouTube API interactions
```

## Setting Up YouTube API 🎥

To access YouTube's data, you'll need to:

1. Create a project in Google Cloud Console
2. Enable the YouTube Data API v3
3. Generate an API key
4. Use the `tuber` package in R to interact with the API

## Data Analysis: Hari Raya Music Videos 📊

Our analysis covers several aspects of Hari Raya music videos:

### Top Performers 🏆

* Top 10 most viewed videos
* Top 10 most liked videos
* Top 10 most commented videos

### Trend Analysis 📈

* Correlation between views, likes, and comments
* Historical ranking of videos (2009-2025)
* Seasonal patterns in engagement

## Limitations and Considerations ⚠️

While working with the YouTube API, we encountered some limitations:

* Search results are limited to short videos
* API quotas and rate limits
* Data freshness and update frequency

## Beyond YouTube: Other API Applications 🌐

The world of APIs offers endless possibilities for data analysis:

* 🌤️ Weather forecasting
* 🎵 Spotify music trends
* 📰 News headline analysis
* 📱 Social media analytics
* 🏛️ Government datasets

## Resources and Further Reading 📚

* [YouTube API Documentation](https://developers.google.com/youtube/v3)
* [Free APIs Collection](https://github.com/public-apis/public-apis)
* [R Package Documentation](https://www.rdocumentation.org/)
* [API Best Practices Guide](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

## Conclusion 🎯

Working with APIs opens up a world of real-time data analysis possibilities. Whether you're analyzing music trends, weather patterns, or social media engagement, APIs provide a powerful way to access and analyze data. I hope this post has inspired you to explore the world of APIs in your data analysis projects.

---

### Thank you! 🙏

Feel free to reach out if you have any questions or would like to discuss API integration in your projects.