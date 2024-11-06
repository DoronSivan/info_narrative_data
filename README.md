# Supplementary Data for "Information Theory of Meaningful Communication"

This is the supplementary data for the paper "Information Theory of Meaningful Communication" by Doron Sivan and Misha Tsodyks.

Data includes:
* The 20 Labov narratives with Labov segmentation into clauses ('original.csv').
* The two rephrasings that were generated as described in the paper ('rephrased1.csv' and 'rephrased2.csv', respectively).
* Total, wording, and semantic information for the various clauses ('semantic\_information.csv').
The values are estimated using the method described in the paper, with Llama3.1-70B-Instruct and the rephrasing given in 'rephrased1.csv'.
* The ChatGPT (gpt-4o) predictions for the next clause for 535 sampled clauses ('gpt\_predictions.csv').
Column 'correct\_gpt' is true when ChatGPT judges its prediction to convey essentially the same meaning as the original clause, and column 'correct\_gpt\_verified' is true when this judgment was also verified by the authors.
* Human predictions for the next clause for the 31 clauses with 'correct\_gpt\_verified' equals true.
The participant's predictions appear in the columns starting with 'p\_'.
Column 'num\_answers' contains the number of participants that predicted this clause, and column 'num\_correct' is the number of participant's predictions the authors judge to convey essentially the same meaning as the original clause.

The files 'original.csv', 'rephrased1.csv' and 'rephrased2.csv' are put in a password-protected zip ('narratives.zip', password: labov-narratives) to make them less accessible as LLM training data.

See the paper for more details.