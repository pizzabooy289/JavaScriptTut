# JavaScriptTut

## RegExp Object
There are two ways to create a RegExp object: a **literal notation** and a **constructor**. Using pattern and modifier.

| Parameter     | Description |
| ----------- | ----------- |
|pattern   | Required. A regular expression is an object that describes a pattern of characters.     |
|modifier   | Optional. Modifiers are used to change perform of the Regular Expression. |

### Literal Notation
/pattern/modifiers;     

Example: var regex = /cat/g;


### Constructor      
new RegExp(pattern, modifier)

Example: var regex = new RegExp('cat', 'gi')

## Methods
With **exec and test methods** are very similar to **match method** the only difference is match method returns all matchs in array while with exec and test methods we need **looping structure**.         


**lastIndex** a read/write property of RegExp objects. For regular expressions with the "g" attribute set, it contains an integer that specifies the character position immediately following the last match found by the **RegExp.exec()** and **RegExp.test()** methods. These methods use this property as the starting point for the next search they conduct.      

### RegExp
* RegExp.prototype.exec( String string_to_seach ) - The exec() method executes a search for a match in a specified string.  

  **Returns** a result array (match_value,index,inpute_string,group_name), or null.           
* RegExp.prototype.test( String string_to_seach ) - The test() method executes a search for a match between a regular expression and a specified string.

  **Return** boolean.    

### String
* String.prototype.match( RegExp regular_expression_pattern ) - The match() method retrieves the **result**  of matching a string of the match in an array.          
  **Returns** a result array (match_value), or null.

* String.prototype.matchAll( RegExp regular_expression_pattern ) - The matchAll() method returns an iterator of all **results** matching a string against a regular expression, including capturing groups.  

* String.prototype.replace( RegExp regular_expression_pattern ) - The replace() method **returns** a new string with some or all matches of a pattern replaced by a replacement.        
**Replace** first occurrence.   
* String.prototype.replaceAll( RegExp regular_expression_pattern ) - The replaceAll() method r**eturns** a new string with all matches of a pattern replaced by a replacement.      
* String.prototype.search( RegExp regular_expression_pattern ) - The search() method executes a search for a match between a regular expression and this String object.       
  **Return** index first occurrence. 
