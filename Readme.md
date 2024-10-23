# League of Legends (LoL) 50,000 Ranked Games Analysis

## Overview
This repository contains an analysis of **50,000 ranked League of Legends (LoL) games** from the EUW region. The dataset provides a comprehensive look at various in-game factors such as team composition, key objectives, and game outcomes. The goal of this analysis is to uncover patterns that influence match outcomes and to explore potential models for predicting game results based on these factors.

## Table of Contents
- [Overview](#overview)
- [Motivation](#motivation)
- [Data Sources](#data-sources)
- [Technologies](#technologies)
- [Project Structure](#project-structure)
- [Analysis Breakdown](#analysis-breakdown)
- [Key Findings](#key-findings)
- [Future Work](#future-work)
- [Contact](#contact)

## Motivation
League of Legends is a popular team-based strategy game, and understanding what contributes to winning or losing a match is critical for both casual and professional players. This project aims to:
- Analyze **50,000 ranked games** to identify the most impactful game factors.
- Build predictive models that can forecast match outcomes.
- Provide insights that can inform both players and game designers.

## Data Sources
The dataset used in this analysis includes over **50,000 ranked EUW games** and provides fields for:
- **Game ID**: Unique identifier for each game.
- **Creation Time**: Timestamp of when the game was created.
- **Game Duration**: The length of the game in seconds.
- **Season ID**: Identifies the season of the match.
- **Match Outcome**: Indicates the winner (1 = team1, 2 = team2).
- **In-Game Events**: First Baron, dragon, tower, blood, inhibitor, and Rift Herald (1 = team1, 2 = team2, 0 = none).
- **Team Composition**: Champions and summoner spells for each team, using Riot's champion and summoner spell IDs.
- **Objective Control**: The number of towers, inhibitors, Baron, dragon, and Rift Herald kills for each team.
- **Champion Bans**: The five champions banned by each team.

The dataset was collected via the Riot Games API, and usernames were scraped from 3rd party LoL sites to gather match data.

**Link to Dataset**: [Kaggle Dataset](https://www.kaggle.com/datasets/datasnaek/league-of-legends)

## Technologies
The following tools and technologies were used in this project:
- **Python**: Core language for data analysis and machine learning.
- **Pandas**: For data manipulation and analysis.
- **Scikit-learn**: For building and evaluating machine learning models.
- **Matplotlib** and **Seaborn**: For data visualization.
- **Pickle**: For saving trained models.
- **Jupyter Notebooks**: For documenting and running the analysis.

## Project Structure
```bash
📂 League_Of_Legends_Games_Analysis_Project
├── 📂 1-Original Data          # Original raw data
├── 📂 2-Prepared Data          # Cleaned and pre-processed data
├── 📂 3-Uploaded Data          # Data ready for analysis
├── 📂 4-Analysis               # Notebooks and scripts for data exploration and model development
│   ├── lol_analysis.ipynb              # Main analysis notebook
│   ├── lol.pkl                         # Pickled machine learning models
│   ├── logs.log                        # Log files for analysis steps
├── 📂 5-Insights               # Key insights and results from the analysis
├── 📂 6-Final                  # Final models and results
├── 📂 Other Files              # Miscellaneous or supporting files
├── README.md                   # Project overview (this file)
├── git_commands.ipynb          # Useful git commands for managing the project
