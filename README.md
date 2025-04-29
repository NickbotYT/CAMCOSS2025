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

  
