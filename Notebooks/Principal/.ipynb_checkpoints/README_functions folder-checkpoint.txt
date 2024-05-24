Here, we'll explain what the different functions of our project do.

## filtering.ipnyb

These functions filter entries in a pandas DataFrame database according to the presence of a specific keyword in a designated column. 
They are particularly useful for isolating specific chemical datas, such as the presence of "Isopropyl" or “Sodium Hydroxide” in the 'Molecule' column.

## newdatabase.ipnyb

These functions allow you to exclude rows from a pandas DataFrame database based on the presence of a specific value in a given column. In our project, they are useful for eliminating creams containing specific bad molecules, and so help to rank and select the best creams.

## ranking_for_pregnancy.ipnyb

By creating dictionaries, these functions have made it possible to rank the various creams in ascending order of their harmfulness to pregnant women. This ranking is based on the number of molecules hazardous to pregnancy.


More details concerning each function can be found in a seperate README file in the "function module".

## visualizing.ipnyb

Using RDKit, this function visualizes the molecules present in a given cream, and colors molecules deemed harmful. Some molecules contain harmful groups, and are only partially colored, since only these groups are colored. However, in this case, the molecules are not really harmful, since the harmful groups are contained in the molecule and not present on their own: their harmful effect is therefore cancelled out, or at least greatly reduced.
Finally, this function posed a problem when it was first created, as Smiles and smarts structures were initially mixed. We therefore ended up using only Smiles structures.