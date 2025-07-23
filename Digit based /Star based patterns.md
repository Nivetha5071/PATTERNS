## DIGIT BASED PATTERNS

## 01.Basic pattern

````java[]

import java.util.*;
public class pattern1 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		for(int row =0;row<n;row++) {
			for(int col =0;col<n;col++) {
				System.out.print(row+1);
			}
			System.out.println();
		}
  }
}
output:
5
11111
22222
33333
44444
55555
````

## 02.
````java[]

import java.util.*;

public class pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		for(int row =0;row<n;row++) {
			for(int col =0;col<=row;col++) {
				System.out.print(row+1);
			}
			System.out.println();
		}

	}

}

output:
1
22
333
4444
55555
````
3.print the numbers pattern in continuous order:
````java[]

import java.util.*;

public class pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		for(int row =0;row<n;row++) {
			for(int col =0;col<n;col++) {
				System.out.print(col+1);
			}
			System.out.println();
		}

	}

}
output:
5
12345
12345
12345
12345
12345
````

4. p
````java[]
 public class pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		int t=1;
		for(int row =0;row<n;row++) {
			for(int col=0;col<n-row-1;col++) {
				System.out.print(" ");
			}
			for(int col =0;col<t;col++) {
				System.out.print(row+1);
			}
			t= t+2;
			System.out.println();
		}

	}

}

output:

5
    1
   222
  33333
 4444444
555555555
````

5.
````java[]
public class swaping {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		//System.out.println(3-n);
		int val;
		for(int row = 0; row<n; row++) {
			val = ((row+1)%2==0)? 2:1;
			for(int col = 0; col<=row;col++) {
				System.out.print(val);
			}
			System.out.println();
		}
	}

}

output:
5
1
22
111
2222
11111
````
6.
````java[]
import java.util.*;
public class swaping {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		//System.out.println(3-n);
		int val;
		for(int row = 0; row<n; row++) {
			val = ((row+1)%2==0)? 2:1;
			for(int col = 0; col<=row;col++) {
				System.out.print(val);
				val = val+2;
			}
			System.out.println();
		}
	}

}

output:
5
1
24
135
2468
13579
````
7.
````java[]
import java.util.*;

public class pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		for(int row = 0; row<n; row++) {
			int val = row+1;
			int diff=n-1;
			for(int col = 0; col<=row;col++) {
				System.out.print(val);
				val= val+diff;
				diff--;
			}
			System.out.println();
		 }
		}

	}

output:
5
1
26
3710
481113
59121415
````

## STAR BASED PATTERNS


1. RIGHT ANGLE TRIANGLE

````java[]

INVERSSE:
public class Solution {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int t= 2*n-1;
        for(int row=0;row<n;row++){
            for(int col=0;col<=row-1;col++){
                System.out.print(" ");
            }
            for(int col=0;col<t;col++){
                System.out.print("*");
            }
            t= t-2;
            System.out.println();
        }
    }
}
output:

*******
 *****
  ***
   *
````
## 2.STRAIGHT:
````java[]

 int n = sc.nextInt();
        int t=1; 
        for(int row=0;row<n;row++){
            for(int col=0;col<n-row-1;col++){
                System.out.print(" ");
            }
            for(int col=0;col<t;col++){
                System.out.print("*");
            }
            t= t+2;
            System.out.println();
        }

output:
   *
  ***
 *****
*******
````

 ## 3.M-> PATTERN:
````java[]
public class pattern1 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        for (int row = 0; row < n; row++) {
            for (int col = 0; col < n; col++) {
                if (col == 0 || col == n - 1 ||( row == col && row<=n/2)||(row+col==n-1 && row<=n/2)){
                    System.out.print("*");
                }
                else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}
OUTPUT:
7
*     *
**   **
* * * *
*  *  *
*     *
*     *
*     *
  ````

## 4.W-> PATTERN:
````java[]
import java.util.*;


public class pattern1 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        for (int row = 0; row < n; row++) {
            for (int col = 0; col < n; col++) {
                if (col == 0 || col == n - 1 ||( row == col && row>=n/2)||(row+col==n-1 && row>=n/2)){
                    System.out.print("*");
                }
                else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}
OUTPUT:
7
*     *
*     *
*     *
*  *  *
* * * *
**   **
*     *
````
## 5.N-> PATTERN:
````java[]
import java.util.*;


public class pattern1 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        for (int row = 0; row < n; row++) {
            for (int col = 0; col < n; col++) {
                if (col == 0 || col == n - 1 || row == col)
                    System.out.print("*");
                else
                    System.out.print(" ");
            }
            System.out.println();
        }
    }
}
OUTPUT:

5

*   *
**  *
* * *
*  **
*   *
````
