The workflow created here does the following:
Retrieves the rows from a previously specified sheet
Filters those with incomplete information
From the filtered rows, it retrieves the ID fields and makes HTTP requests to obtain the corresponding Pokémon information
It uses the Edit Fields node to retrieve only the necessary fields and rename them if required
It updates the rows in the original sheet, matching the IDs
It uses the Aggregate node to convert the multiple results into a list
Using the Send Email node and receiving the list of results, it delivers a report.