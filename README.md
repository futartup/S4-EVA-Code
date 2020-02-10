# S4-EVA-Code

The model:

# Block 1

28 * 28 * 1 | 3 * 3 * 1 * 8 | 28 * 28 * 8. ==> relu + batch normalization
28 * 28 * 8 | 3 * 3 * 8 * 8 | 28 * 28 * 8. ==> relu + batch normalization
28 * 28 * 8 | 3 * 3 * 8 * 8 | 28 * 28 * 8. ==> relu + batch normalization + max pooling + dropout(0.25)

# Block 2

14 * 14 * 8 | 3 * 3 * 8 * 16 | 14 * 14 * 16 ==> relu + batch normalization
14 * 14 * 16 | 3 * 3 * 16 * 16 | 14 * 14 * 16 ==> relu + batch normalization
14 * 14 * 16 | 3 * 3 * 16 * 16 | 14 * 14 * 16 ==> relu + batch normalization + max pooling + dropout(0.25)

# Block 3
 
7 * 7 * 16 | 3 * 3 * 16 * 64 | 7 * 7 * 64 ==> relu + batch normalization + max pooling + dropout(0.25)
7 * 7 * 64 | 1 * 1 * 64 * 10 | 7 * 7 * 10

# GAP Layer

The output of GAP layer is applied to log of softmax function



