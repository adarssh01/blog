---
layout: post
title: "Rotate a given rectangle array by 90 degree clockwise in Java"
subtitle: "Given a rectangle array n×m in size. Rotate it by 90 degrees clockwise, by recording the result into the new array m×n in size."
# date: 2020-01-26 23:45:13 -0400
background: '/img/posts/java.jpg'

---
This program reads in a two-dimensional array from the user, and then creates a new array by rotating the original array by 90 degrees counterclockwise.

``` java
import java.util.Scanner;

class Main {
    
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = scanner.nextInt();
        int m = scanner.nextInt();
        int[][] array = new int[n][m];
        for (int i = 0; i < n; i++) {
            for (int j = 0; j < m; j++) {
                array[i][j] = scanner.nextInt();
            }
        }

        int[][] newArray = new int[m][n];
        for (int i = 0; i < n; i++) {
            for (int j = 0; j < m; j++) {
                newArray[n - i - 1][i]= array[i][j] ;
            }
        }
        for (int i = 0; i < m; i++) {
            for (int j = 0; j < n; j++) {
                System.out.print(newArray[i][j] + " ");
            }
            System.out.println();
        }


    }
}
```
The output of the program will be the rotated array, with each row on a separate line and the elements in each row separated by a space.
For example, if the input is:

```
3 3
1 2 3
4 5 6
7 8 9

```
Then the output will be:

```
7 4 1 
8 5 2 
9 6 3 
```

[Java](https://www.java.com/en/){: .btn}