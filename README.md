
# Pandas 

1. **Dimensionality**

      df.shape()
      
      info()
      
      describe()

2. **Type type(df)**  : USed to check the data type of a column use 

    df['chas'].dtype
    
3. **Slicing and indexing**

    list = [1,2,3,4,5] 

    list[1:3] : start : stop 

    df.iloc[a:b:x:y] a = start and b end of row and x start and y end for cloumn
    df.loc()

4. **Identify unique elements**

    df['cnamd'].unique() // specified column

5. **Value extraction**
    using **value()** on a column return all the values of the column 
    df['crim'].value()

# Statistical module
    1. **Arithematic mean**
      df.mean() 
      
      df.median() // separates higher half of the data from lower half
      
      mode // used to identify the central tendency of numeric or nominal data

      Which can also be used on non numeric data ( the only funciton )

      df.mode(axis=0) // caluclate mode over columns

      df.mode(axis=1) calculated mode over rows
      
# different function of a data object

1.  head()  -- head(3)
2.  tail()
3. values() - // return series of the array 
4. groupby() - //print(df.groupby(['Team', 'Rank']).groups)
5. Concatenation -- join two or more datastructures  
print(pandas.concat([df1,df2], axis=1) )
6. Merging --> need to have a common column between two or more datasets or tables.
print(pandas.merge(df1,df2, on='Team'))

            1. Left join print(pandas.merge(df1,df2, on='Team', how='left'))
            2. right join print(pandas.merge(df1,df2, on='Team', how='right'))
            3. inner join : selects all rows from both table if matching between columns 
            Left join print(pandas.merge(df1,df2, on='Team', how='inner')) // returns null if no match
            4. full outer join -- retrun all when there is a match in left or right
            
  # Type casting 
      string()
      int()
      float()
      implicit --> happens without effor or code 
      Explicit  --> reuse code or DRY programming 
      
      
  
            
            
      
