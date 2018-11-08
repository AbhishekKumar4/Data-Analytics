# Association Rule Mining

- Mining frequent patterns and rules.
- Idea is we want to figure out what kind of entities are frequently co-occuring in inputs. So, we can say that there is some kind of association in these.

**Two Stages**

- Find frequent patterns
  - Stage where we analyze data very closely.
- Association Rules : Conditional dependencies
  - We want to derive assiciation in form that if A occurs than B occurs.
  
  
Difficult part is finding the pattern. Once we find the pattern than deriving association is not that typical.

We could find patterns in :
- Sequences
  - Time series data, fault analysis
- Transactions
  - Market based data
- Graphs
  - Social network analysis
    
# Mining Transactions

- Transaction is a collection of ites brought together.
  - For example :  we go to supermarket and buy items and on checkout make payments. So all the items we bought forms a transactin. **It could be set of items --> Itemset**.
- Goal is to find frequesnt itemsets, so than we can g ahead and form rules.

Itemset A ==>(implies) ItemsetB, if both A and A U B are frequent ietmsets. Example : Milk and Bread.

**Applications of Minings transactions**

- Market Basket Analysis
  - Putting milk and bread together at same place in the supermarket.
- Predicting Co-occurances
- Time series analysis
  - Trigger events


