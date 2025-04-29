# CAMCOSS2025
Example Stackleberg SImulation


This project simulates blockchain-style transaction auctions to analyze how leaders (block proposers) can exploit followers (other users) under different conditions such as:

-Latency (Delay in response)
-Capital Constraints (limits on transaction spending)

We model two types of simulations:

-Exploitation Analysis: How leaders strategically choose moves to maximize their advantage over followers.
-Latency Impact: How leader earnings vary when followers experience delays.

The project generates random transaction data across multiple auction rounds, simulates both leader and follower behavior, and visualizes the results with multiple comparison graphs.
Main Features

-Random Transaction Generation: Each auction has randomly assigned gas and tip amounts.

-Leader and Follower Strategies:

  a)Leader picks optimal moves first.

  b)Follower reacts based on remaining gas and potential latency.

-Capital Limit Simulation: Option to restrict the follower’s total tip size to simulate resource constraints.

-Multiple Rounds: Run hundreds of auctions to observe overall trends.

-Detailed Visualizations:

1)Leader vs Follower earnings comparison

2)Exploitation advantage plots

3)Histograms of earnings distributions

4)Moving average plots

-Comprehensive Summaries: Key statistics (Min, Max, Mean, Median) for each simulation setting.

Data Saving:

All transactions from all rounds are saved to CSV and Excel (auction_data/ folder).

Files

stackleberg.py: Main Python file running the simulation.

files created while running the grogram
-auction_transactions.csv: CSV file containing all transactions round-by-round.
-auction_transactions.xlsx: Excel version of the transaction data.


Usage:
Run the Script
Simply execute stackleberg.py it will automatically:

-Simulate 100 rounds for each configuration.
-Plot and display all comparison graphs.
-Save transaction data.

Dependencies

Python 3.x
Packages:

numpy
pandas
matplotlib
itertools
os
random

Install packages using:

-pip install numpy pandas matplotlib

Output Description

Plots:
-Line plots showing how leader and follower earnings change over time.

-Histograms showing the distribution of earnings and exploitation.

Summaries:

-Text-based min/max/mean/median summaries for exploitation advantages and leader earnings.

Data Files:

-Each transaction is saved along with its round number for easy tracking and future analysis.

Notes

-You can change the number of auction rounds by modifying the rounds parameter in run_multiple_auctions_exploitation and run_multiple_auctions_latency.
-delay_factor controls how likely a follower makes suboptimal decisions due to network delays.
-capital_limit simulates a financial constraint on the follower’s ability to maximize tips.
  
