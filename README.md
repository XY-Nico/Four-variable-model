# Four-variable-model
四变量模型

Through the method of full arrangement, possible four-variable models are found. Currently, the models that have been realized include 
                      M1: mediation model with regulating effect
                      M2: regulation model with mediating effect
                      M3: multiple mediation model
通过全排列的方法，找到可能的四变量模型，目前已经实现的模型有M1有中介的调节模型，M2有调节的中介模型，M3多重中介模型

method of application 
使用方法

data table:the name of Var is like A1(means the first scale's total score)
                                   A2(means the second scale's total score)
                                   A3_1(means the first dimensionality of the third scale's toal score)
              e.g.   ID     A1_1    A1_2    A1     A2_1      A2_2    A2_3     A2     A3     A4
                     01       11     25     36      5         8       13      26     34     48
                     01       23     22     45      11        2       13      28     36     62
                     01       12     13     25      7         1       8       14     32     54
                     01       32     35     67      4         5       9       33     30     57
                     01       14     27     41      7         7       14      19     22     61
       WARNING!!!:you need save the data table in '.xlsx'(Excel 2010+),if not you need to change the second code to read your data!
***IF everything is well***
  First,Marks the variable to be evaluated in the fourth code:  listVar = c()
    e.g. if you want to run the A1,A2,A3,A5,A6,A7,A9
            you need to full the listVar like:    listVar = c(1,2,3,5,6,7,9) or listVar = c(1:3,5:7,9)
         and if you want to run the A1_1,A1_2,A1_3,A4
            you need to full the listVar like:    listVar = c(1.1,1.2,1.3,4)
  Then,you can run all the code and get a result named 'O.xlsx'.It will give you a result about all the possibility!And you can find the path in the table WITH THEORY! 
  The result is only gotten by data without any THEORY!Please check the theory first!
  
  the output table's sample
                            I	J	K	L	 M1 M2 M3
                        23	2	4	3	7	 0  0	 0
                        24	2	4	3	8	 0  0	 0
                        25	2	4	5	3	 0  0  0
                        26	2	4	5	6	 0  1  0
                        27	2	4	5	7	 1  1  0
                        28	2	4	5	8	 0  1	 1
                        29	2	4	6	3  0  0  0
                        30	2	4	6	5	 0  1	 1
                        31	2	4	6	7  0  0  0
                        32	2	4	6	8	 0  1	 0
the first row means the ID of the result (instead of the subject's !!!)
the second row(I) means the first Var's ID (dependent variable)
the third row(J) means the second Var's ID (mediating variable)
the fourth row(K) means the third Var's ID (regulating variable)
the fifth row(L) means the fourth Var's ID (independent variable)
  M1: mediation model with regulating effect
  M2: regulation model with mediating effect
  M3: multiple mediation model(both J and K are mediating variable)
        
