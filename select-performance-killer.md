# Select (Performance Killer) working with functions in where 

## Example 

```
explain select * from actor where last_name like concat(substring(first_name,1,1),'%');
```

## Das ist kein Problem  

```
explain select substring(first_name,1,1) from actor where last_name like 'L%';
```
