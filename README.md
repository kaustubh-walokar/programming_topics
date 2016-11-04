# Topics

## Recursion

1. CS106B Stanford - Programming Abstractions
    * [Lecture 9](https://www.youtube.com/watch?v=uFJhEPrbycQ)
        ```java
        public static void permutation(String str) { 
            permutation("", str); 
        }
        
        private static void permutation(String prefix, String str) {
            int n = str.length();
            if (n == 0) System.out.println(prefix);
            else {
                for (int i = 0; i < n; i++)
                    permutation(prefix + str.charAt(i), str.substring(0, i) + str.substring(i+1, n));
            }
        }
       ```
    * [Lecture 10](https://youtu.be/NdF1QDTRkck)
    ```java
            public static void combinations(String str) { 
                combinations("", str); 
            }
            
            private static void combinations(String prefix, String str) {
                int n = str.length();
                if (n == 0) System.out.println(prefix);
                else {
                     combination(prefix + str.charAt(i), str.substring(i));
                     combination(prefix , str.substring(i));
                }
            }
    ```

## Hashing
1. [CS006 MIT - Introduction To Algorithms](https://www.youtube.com/watch?v=HtSuA80QTyo&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
    * Lecture 7
    * Lecture 8
    * Lecture 9