# EachRowColumnSum-Java_interview_practice
Java program to calculate the sum of each row and column in 2-d array
package com.rowColumn;

/**
 *
 * @author Dinesh Nanda
 */
public class EachRowColumnSum {

    public static void main(String[] args) {

        int arr[][] = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
        
        int rows = arr.length;
        int cols = arr[0].length;
        
        int row_sum = 0;
        int col_sum = 0;
        
        
        for (int i = 0; i < rows; i++) {
            row_sum=0;
            for (int j = 0; j < cols; j++) {
                
                row_sum = row_sum + arr[i][j];
          
            }
            System.out.println("Sum of "+(i+1)+ " row: "+ row_sum);
        }
        
        for (int i = 0; i < cols; i++) {
            col_sum=0;
            for (int j = 0; j < rows; j++) {
                
                col_sum = col_sum + arr[j][i];
          
            }
            System.out.println("Sum of "+(i+1)+ " column: "+ col_sum);
        }

    }
}
