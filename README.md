# belief_neglect
All code and data used in the belief neglect project.

## Structure
You can find the data and analysis scripts for study 1 and study 2 under the folders "study1" and "study2", respectively. 

Inside each folder, you'll find the data under "data/study{X}_cleaned_data.csv".

Inside the data, column names are as follows:
- ```Participant_id```: Unique ID of each participant.
- ```Duration```: Duration (in seconds) that the participant took to complete the experiment.
- ```Group``` [Study 2 only]: Group that the participant was assigned to in the experiment. This can take the values of: ```1``` (Relevance training group), ```2``` (Irrelevance training group) or ```3``` (no training group).
- ```Test```: Test question ID. The values of ```TEST_S1_P_1```, ```TEST_S2_P_1```, and ```TEST_S3_P_1``` are assigned to the three test questions. The value of```TEST_S1_P_val_1``` denoted the validation question. The questions were displayed as: "Based on the demonstration, what do you think is the probability (0%-100%) that the following statement is true? This person prefers Yellow diamond over Red diamond". The questions were presented in a randomized order.
- ```Test_Score```: Participant response to the question in the ```Test``` column.
- ```is_val```: Binary variable denoting a validation question. ```1``` if it is a validation question, ```0``` otherwise.

## Analysis
The analysis of the data can be found in the ```study{X}_analysis.Rmd``` file, which uses the R Markdown format.
