![AW-1](https://user-images.githubusercontent.com/23423475/193085886-f4753690-7b9c-4d54-988f-1dc176a568ab.JPG)
![AW-2](https://user-images.githubusercontent.com/23423475/193085895-062a8371-f2a9-4f87-94b2-530ff79c4c6d.JPG)
![AW-3](https://user-images.githubusercontent.com/23423475/193085900-c8228270-5e0a-40f9-9ef1-2a30254d9e73.JPG)
==============================================================================================================================================
Learning:
 1. Intro to Power BI Ecosystem, PBI Desktop, PBI Services.
 2. BI Concepts.
 3. Power BI Architecture.
 4. Power BI interface tour.
 5. Connecting PBI with different data sources.
 6. Benefit of connecting with a folder. If we connect to single individual file, we have to append them to create a single data file, e.g. sales file for different years, also when we will get a new file for next year, we have to manually load that file every time. this is only applicable with similar type of files. When we directly connect with a file, we create an endpoint or bridge of data between pbi and that particular file, so in future even if there is a slight change with the name of the file, that bridge will collapse, connection will break because if wont be able to find or read the other endpoint with that similar name.
 7. Data transformation through Power Query:
 8. Transform vs Add column.
 9. After loading data, 1st step is always to check data type of every column.
 10. Categorizing table as fact or dim.
 11. add,merge, remove column.
 12. Renaming recorded steps, to indentify later which step does what.
 13. Multi level sorting.
 14. Merge query vs append query.
 15. Merge query - adding new columns.
 16. Append query - adding new rows.
 17. Merging query - we have product key available, but we dont have product cost, so if we have to fetch cost over here, first we have to connect with relevant table also. it is kind of visual vlookup.
 18. now, every cell of column has a link with table, means entire table in itself, because we mentoned from which table we need values, but we did not mentioned which column of that table we needed over here, so it linked the entire table.
 19. although, it is recommended to create relationships between table and bring the data, rather that merging.
 20. group by - in the end, if we do close and apply, only these few grouped values will be loaded into our data model, and not the entire table.
 21. pivot unpivot columns.
 22. Splitting values.
 23. Text before delimiter.
 24. Building calendar table.
 25. Conditional column.
 26. Custom column.
 27. Invoke custom column.
 28. Data modelling: understanding relationship, cardinality.
 29. Filter flow and cross filter direction.
 30. We can have multiple relationship between table, but only 1 active relation at a time.
 31. DAX: Calculated Column vs Measure
 32. Logical DAX - IF/AND
 33. Switch
 34. Relational functions
 35. Related: to bring data from dimension to fact table
 36. Relatedtable: to bring data from fact to dimension table. It gave answer, but answer remained same throughout, it is showing us total order qty sold, because it is not recognizing the product key within the row, it is simply doing sum of entire qty sold
 37. Filter and row context
 38. The entire total order qty got filtered, based on the item we put, they are reacting to filter context, but this will only work if there is a relation within the tables, so what it is doing in background is that it goes back to tables, and filter out the result basis on what we put in field
 39. Creating table from scratch, and keeping all measures in it
 40. Count fx
 41. Calculate fx
 42. Building calculated table using filter function
 43. Variables in fx
 44. Sameperiodlastyear
 45. Iterator functions
 46. Crossfilter - Sometimes we need to fetch value from indirectly related table, e.g. cust and territory table are not related directly, suppose I want to know, in which country what is the avg annual income of our customers. requirement is terr table should be able to control customers table, but right now it can control only sales table, but further sales cannot control customers table because from sales filter is not flowing towards cust table. we can go into properties of data modelling and change filter direction to cross filter, but it will create lot of issues with rest of the dataset and model.
 47. ALL - Ignore filter context
 48. YTD calculation
