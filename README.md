
### Beat the BTB with vowpall wabbit

1. Run csv2vw.py to read the data into the right format. You'll need to change the path of each file for this

The output file has a namespace for each variable, in order to allow making interactions more flexible.

#### add - display
|a ad_id |b display_id
#### events
|u uuid|d document_id|p promoted|c country|s state|l localoty|w week|h hour|
#### promoted
|x document_id |y campaign_id |z advertiser_id

2. `vwcommands.sh` has an example of the model I've used to get to 0.64144 in the public leaderboard, that by this time is at the 90th position. 
Not great but a nice start with room for improvement.
The average loss for this model is: 0.437686

3. write_submission.R converts the output of vw into probabilities, and finally the submission format. 

See this notebook for more details:
https://martinbel.github.io/outbrain-click-prediction-with-vowpal-wabbit.html 
