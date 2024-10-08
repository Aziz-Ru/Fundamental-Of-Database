# Relational Algebra

Relational Algebra is a procedural query language. Relational algebra mainly provides a theoretical foundation for relational databases and SQL.

These are the **basic/fundamental operators** used in Relational Algebra.

  - Selection(σ)
  - Projection(π)
  - Union(U)
  - Set Difference(-)
  - Set Intersection(∩)
  - Rename(ρ)
  - Cartesian Product(X)
    
### Selection(σ)
It is used to select required tuples of the relations.we allow comparisons using =, =, <, ≤, >, and ≥ in the selection predicate. Furthermore, we can combine several predicates into a larger predicate by using the connectives and (∧), or (∨), and not (¬). **In relational algebra, the term select corresponds to what we refer to in SQL as where.**

###  Projection(π)
It is used to project required column data from a relation. **This is alway return unique.In relational algebra, the term project corresponds to what we refer to in SQL as select.**

### Union(U)
Union operation in relational algebra is the same as union operation in set theory.The only constraint in the union of two relations is that both relations must have the same set of Attributes.  

### Set Difference(-)
Set Difference in relational algebra is the same set difference operation as in set theory.The expression r − s produces a relation containing those tuples in r but not in s. The only constraint in the Set Difference between two relations is that both relations must have the same set of Attributes.  

### Curtesian Product
The Cartesian-product operation, denoted by a cross (×), allows us to combine information from any two relations. We write the Cartesian product of relations
r1 and r2 as r1 × r2 .If A has n tuples and a columns and B has m tuples and b columns,in catesian product total tuples =n*m and columns = (a+b).

## Derived Operators
These are some of the derived operators, which are derived from the fundamental operators.** In Question When it say relation of Every or All that must be derived operator.

  - Natural Join(⋈)
  - Conditional Join
  - Intersection (∩)

### Natural Join(⋈)
Natural join is a binary operator. Natural join between two or more relations will result in a set of all combinations of tuples where they have an equal common attribute. 
