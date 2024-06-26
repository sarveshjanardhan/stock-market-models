Data Source
https://www.dropbox.com/scl/fo/qb1i3zi4vuqj4yk49b5f6/ALIafzCpfXsp3yyIHbObjQI?rlkey=wrlti8m48tpjvduz8okuzxa66&e=1&dl=0 

Data Preperation:
preporcess.py --> multiples csv files --> combined_file.csv --> data cleanup in google sheets --> "high" price (labels) add using google finance api --> data.csv (final data used for training)

Model:
Input (input_shape) --> [Dense (64) - ReLU] --> [Dropout (0.5)] --> [Dense (64) - ReLU] --> [Dropout (0.5) --> [Dense (1)] --> Output (1)

Results:
for completely unseeen data on a given day for nifty 50 stocks,
got around avg error of 6% in predictions made using the model and actual highs.
