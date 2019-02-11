# learningSQL  
#### Purpose of this repo: notes on learning SQL  
##### Source: [http://www.sqlcourse.com](http://www.sqlcourse.com)

## Selecting data  

* Structure:
    - select _columnName1_, _columnName2_ from _tableName_ where _columnName_ LOGICAL _stringInSingleQuotes_

* select any column: use *
* select any row: don't include the where statement
* logicals:  
    - =, >, <, >=, <=
    - Not equal to: <>
    - Contains: LIKE

## Creating tables

* Structure:
    - create table _tableName_ (_columnName1_ dataType1(constraint), _columName2_ dataType2(constraint))

* Common data types:
    - char(size): fixed-length character string of length 'size'
    - varchar(size): variable-length character string of maximum length 'size'
    - number(size): number value with maximum length 'size'
    - number(size,d): number value with maximum total length 'size', and maximum number of decimal places 'd'
    - date: date value
    
## Adding records

* Structure:
    - insert into _tableName_ (_list of column names_) values (_list of corresponding values_)
    - there is a space in 'values ()'
    - all strings enclosed in single quotes

## Updating existing records

* Structure:
    - update _tableName_ set _columnName1_ = _newValue1_, _columnName2_ = _newValue2_ where _columnName3_ = _'string'_
    - the new value can be a forumla (e.g. _age + 1_)
