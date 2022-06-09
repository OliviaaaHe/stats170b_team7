# stats170b_team7

## File #1: extract_full_youtube_transcription.ipynb

This is the file to generate the video id, state, date, and full transcript from Youtube API. It will take a long time to run the code due to the length and the amount of the videos, so I put every generated data files (partial data because the original file exceeds 20M) inside already. There's no need to run this file, and the final result for this file is: id_state_date_full_final.csv.

## File #2: extract_portion_youtube_transcription.ipynb

This is the file to generate the video id, state, date, and portion transcript from Youtube API. Instead of generating the full transcript, it only keeps the portion that relates with our topic. This file takes some time to run as well. The generated final result from this result is: id_state_date_portion_final.csv. 

## File #3: google_transcript.py

This file is to extract the transcript from Google Speech-to-Text API. Inside the file, it uses an example of one of the videos we uploaded to Google Cloud.

## File #4: word_error_rate.py

This file is to calculate the word error rate (WER) between two paragraphs/sentences. In the last line, it includes two simple sentences just as an example due to the length of our actual texts. If want to change the texting content, just need to change the contents in the last printing command.

## File #5: meta_data_cleaning.py

Due to the difficulty in reading dates from the first two files, this file will get the dates and transform the dates into consecutive natural numbers. Other elements/metadata are already been generated inside the first two files.

## File #6: finalizing_data.sql

This is an SQL file to clean the invalid data, eliminat empty cells, and combine the above data into one CSV file.

## File #7: modeling.rmd

This is the modeling file using R. We used the structual topic modeling (stm) library inside R to build our model. Along with multiple visualizations inside the file. This file also takes a long time to generate graphs due to the amount of the words inside our database.
