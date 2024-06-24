1. What are the different aspects of the waterfall model?
2. What are the deliverables of the waterfall model?
3. What is the rapid prototype model?
4. What is the iterative model?
5. What are Tront's four principles?
6. What does it mean to require visibility?
7. Why are analysts necessary?
8. What are the difficulties present in the process of analysis?
9. What are the steps in the analysis process?
10. What is the difference between 1NF, 2NF, and 3NF? Give examples
11. What are DeMarco's three views?
12. What are the three levels of specification rigor?
13. What is a model?
14. What is formalization?
15. What are the benefits of a finite state machine?
16. Why is OOA preferred?
17. What is scope of control?
18. What is scope of decision?
19. What is design info hiding?
20. What is coupling?
21. What is cohesion?
22. What is a call graph?
23. What is fan-in/fan-out?
24. What is roll-up?
25. What is roll-down?
26. What is the split implementation strategy?
26. What are the five degrees of scope?
27. What are the four degrees of persistence?
28. What are the three forms of scenario control?
29. What is the definition of design?
30. What is purity?
31. What is completeness?
32. What is data abstraction?
33. What is control abstraction?
34. What is fan-in?
35. What is fan-out?
36. What are the three ways to handle exceptions?


Ask Russell about scope of effect:
If the decision of a function can impact the results it outputs to another 
function, which then uses that as input to calculate a value for another 
function and so on, could the scope of effect not include the majority of the 
call graph?

Example midterm question:
Insert data into the table which demonstrate redundancy
Does this relation prevent duplicates?
Change 1NF to 2NF
Explain all normal forms

5:
Keep it simple
Expect change
Never underestimate
Require visibility

6:
Requiring visibility means that you know what is currently being done in the 
project. With the latest information about the project, estimates can be 
improved, action can be taken if needed, new members can be advised correctly,
and other departments can be accurately informed.

10:
1NF aims to have all tuples of a relation be of the same length, regardless of 
unneeded information being repeated multiple times.

2NF removes the partial key dependencies from the tuples in 1NF by constructing 
new relations where the key in each relation is not compound.

3NF removes transitive key dependencies by adding more relations which contain the 
non-candidate key attribute that is determined by another non-candidate key attribute.

Example:
Recipes(title, recipe_id, author, publication_date)

Chefs(name, chef_id)

Ingredients(name, ingredient_id, price)

|title | recipe_id | author | publication_date | name | chef_id | name | ingredient_id | price|
| ---- |-----------|--------| ---- | ---- | --- | --- | --- | ---|
|Chocolate bark | 5 | A | 2024    | John | 1 | Olive oil | 2 | 2.6|

This is a table in 1NF since we have resolved the issue of recipes having 
differing numbers of ingredients by listing out each ingredient for each 
recipe

The key for this table is recipe_id, chef_id, and ingredient_id.

For the partial key dependencies, we have that name depends on chef_id and 
that the ingredient name and price depend on the ingredient_id. We can 
then separate the table into the three relations listed above.

Furthermore, since none of the non-key attributes in any of the new relations
determine any other attribute, our relations are in 3NF.

11:
DeMarco's three views are the retained data model, the functional model,
and the state transition model. The retained data model demonstrates the 
relationships between the data types. The functional model shows how data is 
passed through and modified. The state transition model reveals what must 
occur in order to move from one state to another.

12: 
The three levels are natural language, diagrams/formal language, and 
formal techniques (BNF, relational algebra, syntax diagrams)

16:
It is natural to how humans think, maps well to OO design patterns. 
OO designs are more likely to be stable after 10 years.

17:
Scope of control are all the items below a specific item in the call graph

24: 
Roll-up is the method of storing entities in only one file, where 
each tuple has the information of the base entity in addition to all the 
attributes of all the derived entities.

20:
Coupling is a measure of how dependent two things are on each other, in 
terms of assumptions or dependencies.

25: 
Each entity is stored in its unique file, containing the attributes 
relevant only to that entity

26: 
You have the entities separated, but the most generic entity has a type 
discriminator

27: 
The four degrees of persistence are:
function or block lifetime
heap lifetime
file lifetime
program lifetime

30: 
Purity means that there are only functions/types/etc... relating to what 
you are constructing

31:
Completeness is when something has everything it needs. E.g., a sequence 
having next, first, and rest.

36:
The three ways are returning/setting a value to indicate an error occurred,
using an error handling function, and throwing exceptions.