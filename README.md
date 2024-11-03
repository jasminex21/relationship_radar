# Realtionship Radar

### Aim
The aim of **Relationship Radar** is to track the progression of a relationship via text message data. This can offer meaningful insights into the evolution of a relationship - e.g., whether a relationship has fizzled out vs grown stronger over time. 

The outlined aim can be addressed by: 
* Collecting text message data and converting it to a standardized format (CSV)
  * Datetime
  * Sender
  * Message content
  * Reply to
* Determine reply times
* Assign each message sentiment scores - maybe using VADER
* Possibly use emotion classifiers to detect emotions from each message
* Identification of trends and patterns in keywords
  * Word frequencies
  * Frequencies of love-related vocab vs words that may indicate conflict
* Topic modeling - I haven't done this before but it would be cool. What are common themes during each stage of the relationship?

To actually investigate a relationship's progression over time, we can look at the above sources of data over window frames (e.g. 5 days, 1 week, etc.). Changes in positive/negative/neutral sentiment over time (can be plotted using line graph)? Word clouds can be used to visualize word frequencies (words can be colored by whether they are positive or negative perhaps). 

And as a nice touch, we can integrate an LLM that is shown the trends and can provide suggestions as to what the best next steps for the relationship are. If it sees a decline in positive sentiment and a rise in negative and neutral sentiment, as well as an increase in reply times, then it might suggest better communication and more quality time.