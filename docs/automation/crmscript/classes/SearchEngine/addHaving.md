---
title: Void addHaving(String field, String compOperator, String value, String rowOperator, Integer priority)
path: /EJScript/Classes/SearchEngine/member functions/Void addHaving(String field, String compOperator, String value, String rowOperator, Integer priority)
intellisense: 1
classref: 1
sortOrder: 9012
keywords: addHaving(String,String,String,String,Integer)
---

Adds a having-clause to the database-query


* **field:** The field to make a restiction on (must also be in group-clause)
* **compOperator:** Comparison operator. Possible values:
OperatorEquals, OperatorNotEquals, OperatorLt, OperatorLte, OperatorGt,
OperatorGte, OperatorLike, OperatorNotLike, OperatorContains,
OperatorBeginsWith, OperatorEndsWith, OperatorIn, OperatorNotIn,
OperatorIs, OperatorOracleLeftJoin, OperatorIsNot
* **value:** The value to be compared with the field
* **rowOperator:** Operator for composing this criteria with a following
criteria
   
**Possible values**   
OperatorAnd, OperatorOr, OperatorNotAnd, OperatorNotOr
* **priority:** A number. All criterias with the same number will be placed
inside
the same brackets


