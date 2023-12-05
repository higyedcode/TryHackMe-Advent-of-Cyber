	Data Science 101 && Jupyter notebooks
	
Intro to pandas
	In pandas, a series is a dictionary of index-value pairs.
	A DataFrame is like a spreadsheet or a database. (esentially a grouping of series)  - or like a matrix
Commands:
	import pandas as pd
	a = ['a','b','c']
	a_series = pd.Series(a)
	
	data = [['Ben', 24, 'United Kingdom'], ['Jacob', 32, 'United States of America'], ['Alice', 19, 'Germany']]
	df = pd.DataFrame(data, columns=['Name','Age','Country'](
	df # this prints the dataframe
	df.count() ; how many opackets were captured
	df["Source"].size()
	df.["Protocol"].value_counts()
	

Matplotlib intro

	from myplotlib import plt
	plt.plot(X,Y) - ex: plt.plot(['Jan','Feb','Mar','Apr'],[8,13,23,40])
		

