---
title: Void addCriteria(String field, String function, String compOperator, String value, String rowOperator, Integer priority)
path: /EJScript/Classes/SearchEngine/member functions/Void addCriteria(String field, String function, String compOperator, String value, String rowOperator, Integer priority)
intellisense: 1
classref: 1
sortOrder: 9004
keywords: addCriteria(String,String,String,String,String,Integer)
---


Adds a criteria on a function of a database-field to the database query




* **field:** The field to make a restiction on
* **field:** The function to use on the field. Possible values:
    FuncCount, FuncAvg, FuncSum, FuncMax, FuncMin, FuncHour,
    FuncWDay, FuncUpper, FuncLower
* **compOperator:**  Comparison operator. Possible values:
  OperatorEquals, OperatorNotEquals, OperatorLt, OperatorLte, OperatorGt,
  OperatorGte, OperatorLike, OperatorNotLike, OperatorContains,
  OperatorBeginsWith,  OperatorEndsWith,  OperatorIn, OperatorNotIn,
  OperatorIs,  OperatorOracleLeftJoin, OperatorIsNot
* **value:** The value to be compared with the field
* **rowOperator:** Operator for composing this criteria with a following criteria
  Possible values
  OperatorAnd, OperatorOr, OperatorNotAnd, OperatorNotOr
* **priority:** A number. All criterias with the same number will be placed inside
   the same brackets


