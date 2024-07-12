# **Power-BI**

## **DAX** - Data Analysis Expressions

DAX is a library of functions and operators that can be combined to build formulas and Expressions used by Microsoft BI tools.
DAX is also known as Function language, where the full code is kept inside a function.

### **Purpose OF DAX** 
  Calculated Columns
  Measures
  Calculated tables

### **Calculated Column  VS Measure**

  ### **Calculated Column**
    Expands the Table by creating a new column
    Stored along with table, consumes memory
    Less Analytical capability

  ### **Measure**
    Summarises data into a single value
    Calculated at runtime / Stored temporarily
    Rich Analytical capability

  ### **Calculated Table**
    Date tables
    Role-playing Dimensions - Individual dimension (Date) playing a main role
    what-if-analysis
    Derived table

  ### **Operators**
    & Concatenation
    && AND Operator
    || OR Operator

### **Naming**

  Table Name   - Sales
  
  Table Name   - 'Canada Sales'
  
  Fully qualified column name - Sales[amount]

### **Data Type**

  DateTime, Date, Time
  
  Text
  
  Whole, Decimal
  
  Boolean

### **Row Context VS Filter Context**

  ### Row Context

    Row context calculates each row, with the values within that row.
    Profit = SUMX(Sales, [Sales Amount] - [Cost Amount])

  ### Filter Context

    Filter context is, a set of filters applied before that table arrives for use.
    Total Sales = SUM(Sales[Sales Amount])

    Applying filters from Filter Pane / Visuals / Slicers
    
### **Calculate**

  Evaluates an expression in a context modified by filters

  Total India Sales = Calculate(SUM(Sales),country = 'India')

  Total Sales = Calculate(SUM(Sales),ALL(country)


### **DAX Functions**
  
  Aggregation functions
  
  Date and time functions
  
  Time Intelligence functions
  
  Filter functions
  
  Financial functions
  
  Information functions
  
  Logical functions

  
  
  
  
  
    


