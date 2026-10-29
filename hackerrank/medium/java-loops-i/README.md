# Java Loops II

![Difficulty](https://img.shields.io/badge/Difficulty-Medium-yellow)

## Problem

**Objective**	
In this challenge, we're going to use loops to help us do some simple math.

**Task**	
Given an integer, $N$, print its first $10$ multiples. Each multiple $N \times i$ (where $1 \le i \le 10$) should be printed on a new line in the form: `N x i = result`.

**Input Format**

A single integer, $N$.

**Constraints**

- $2 \le N \le 20$

**Output Format**

Print $10$ lines of output; each line $i$ (where $1 \le i \le 10$) contains the $result$ of $N \times i$ in the form: 	
`N x i = result`.

## Solution

**Language:** Java  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-10-29T10:42:33.303Z  

```java
import java.util.Scanner;

public class Solution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int q = sc.nextInt();

        for (int i = 0; i < q; i++) {
            int a = sc.nextInt();
            int b = sc.nextInt();
            int n = sc.nextInt();

            int sum = a;

            for (int j = 0; j < n; j++) {
                sum += (int) Math.pow(2, j) * b;
                System.out.print(sum + " ");
            }

            System.out.println();
        }

        sc.close();
    }
}

```

---

[View on HackerRank](https://www.hackerrank.com/challenges/java-loops-i/problem)