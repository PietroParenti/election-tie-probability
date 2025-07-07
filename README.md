# Election Tie Probability

This repository contains a simple Excel model that estimates the probability of a tie in an election with two candidates, assuming each voter votes independently and randomly. The model uses the binomial distribution to compute the likelihood that both candidates receive exactly the same number of votes.

## Key Features

- Calculates the exact probability of a tie in an election with any given number of voters.
- Shows how quickly the probability of a tie decreases as the number of voters increases.
- Based entirely in Microsoft Excel — no coding required.

## Why?

Even though elections can be decided by extremely narrow margins, an actual tie is exceptionally rare. This model demonstrates just how unlikely a tie becomes as the electorate grows. For instance, with 1,000 voters, the probability of a tie is already vanishingly small.

## Excel Limitations

Due to limitations in Excel's numerical precision, the model can no longer compute exact probabilities for large electorates. Specifically:

- Starting from **2048 voters**, the number of combinations (binomial coefficients) exceeds Excel's numeric precision.
- Excel truncates all numbers to 15 significant digits. In other words, 9,999,999,999,999,999 (which is 1×10¹⁶ − 1) is the largest integer that Excel can store without losing precision. 
- As a result, the computed probability is **approximated arbitrarily as zero** for large values of voters — which, in practical terms, is still accurate since the real probability is astronomically small.

This doesn't affect the usefulness of the model, as the chance of a tie at that scale is so close to zero it becomes negligible.
