# RNN_DKT

This is my implementation of the paper: Piech, C., Bassen, J., Huang, J., Ganguli, S., Sahami, M., Guibas, L. J., & Sohl-Dickstein, J. (2015). Deep knowledge tracing (Available: http://papers.nips.cc/paper/5654-deep-knowledge-tracing.pdf) , in Advances in Neural Information Processing Systems (pp. 505-513).

Here, we build an RNN model to predict student learning. We use RNN (specifically Long Short Term Memory (LSTM) model) to predict student responses at an instance  t+1, given all the previous instances.

Here is a description of various files:
1. *rnn_edu.py*: Python code to build and train the RNN model.
2. *skill_builder_data_corrected.csv*: The dataset file from ASSISTments, described here (Links to an external site.)Links to an external site.
3. *correct.tsv*:	A one row per-student file containing the first 100 responses of students in ASSISTments only including students who had 100 or more responses in the dataset.
4. *skill.tsv*:	A one row per-student file containing the skill ID (id created by the preprocessing) of the first 100 responses of students in ASSISTments only including students who had 100 or more responses in the dataset.
5. *assistment_id.tsv*:	A one row per-student file containing the skill of the first 100 responses of students in ASSISTments only including students who had 100 or more responses in the dataset.
6. *skill_dict.json*:	A json lookup-table between the skill ID in skill.tsv and the English language name of the skill.
