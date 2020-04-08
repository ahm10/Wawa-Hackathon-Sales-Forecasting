Background: Robert is an experienced General Manager (GM) of a Wawa in Maryland.
He has a problem – he doesn’t understand the volatility in his stores’ sales of
Product X. He knows that sales per day vary depending on the day of the week
from the automated reporting he receives. But even comparing his store’s sales
on several consecutive Fridays, he notices significant differences that he can't
explain. Robert needs a way to understand what else is going on here, and what,
if anything, he can do about it.

Objectives:

	1.	Find a way to predict future sales at a store level each of the stores
	contained in the dataset provided.

	2.	Produce visualizations that illustrate the impact of relevant factors on
	each store's performance. The visualizations must convey this important
	information in a clear and concise manner, so that Robert can spend his time
	managing the store.

	3.	Find any meaningful patterns in the factors that impact the stores. This
	component is open to the creativity of the participants, and may include
	models, visualization, or both.

Measures of Success:

	1.	The quality of the predictions will be judged by Mean Average Percent
	Error (MAPE) on a holdout sample. After calculating the MAPE for each store,
	we will average them to create a final score which will be used to rank
	participants. A 365 day period will be withheld for this purpose.

	2.	The visualization output will be judged subjectively by the clarity and
	ease with which a non-technical user can interpret them and understand the
	implied impact of each of the factors.

	3.	Objective 3 will be judged by the degree to which participants are able to
	find interesting patterns in the data, especially those that might be
	unexpected!

Rules:

	1.	Tools, techniques, and data:

		a.	Participants may use any datasets, as long as they are publicly
		available at no cost. We encourage you to be creative in the external data
		you consider! If any data not provided by us is used, submissions must
		include a list of those sources (see details below). Anyone using data that
		does not meet these requirements, or failing to disclose the use of such a
		data source will be disqualified.

		b.	Participants may use any programming language or techniques, as long as
		both are available at no cost to any participant.

	2.	Submissions:

		a.	The submission must be made as a zip file. The file name should be
		"<name><lucky number>.zip", where <name> is the participant's full name, and
		<lucky number> is any number of the participant's choosing. The lucky number
		will help resolve any issues arising from two participants having the same
		first and last name.

		b.	All source code should be included in the zip file, in a folder named
		"src".

		c.	The model predictions must be provided in a CSV named "submission.csv",
		with a header line and three fields - "store_number", "date", and
		"sales_index_predicted", that that order. The predictions should include all
		stores, and all dates from 2018-09-22 through and including 2019-09-22.

		d.	A file named "external_sources.txt" must be included if any external
		sources as defined above were used. If none were used, participants should
		include an empty file. Links to each source must be provided.

		e.	Visualizations should be provided in JPG, PNG, or BMP formats. They
		should be placed in a folder named "vis".

		f.	A file named "method.txt" must be included. It should outline the
		approach taken to solve the problem, with brief summary of methods used.

		g.	A file named "patterns.txt" will be included. This file should contain a
		summary of patterns identified (see Objective 3). If visualizations are
		needed to describe the patterns, please include them in the "vis" folder and
		name the images so that they can be easily identified.

Data Provided: In addition to this README, 3 files are provided for your use.

	1.	sales.csv - Contains historical sales (sales_index) and price
	(price_index) for Wawa stores in MD. Measures have been taken to obscure
	actual sales and price while leaving the the relationships in the data intact.
	Sales in this file end on 2018-09-21, but price_index is provided for all
	dates through 2019-09-22 so that prediction is possible. You will notice that some stores
	have missing price_index data during the prediction period. When making predictions, please
	leave those values empty. They will not be counted toward during the evaluation.

	2.	remodels.csv - Contains a list of stores in MD that were closed
	temporarily for remodel, with the start and end dates.

	3.	stores.csv - Contains information about each store in MD, including
	location, store size, and open date.
