# Reverse_String
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String A=sc.next();
        StringBuilder sb=new StringBuilder();
       sb.append(A);
       sb.reverse();
       if(isPalindrome(A)){
          System.out.println("Yes"); 
       }
       else{
           System.out.println("No");
       }
    }
    public static boolean isPalindrome(String A){
        int n=A.length();
       for (int i = 0; i< n/2;i++) {
            if (A.charAt(i) != A.charAt(n - i - 1)) {
                return false;
            }
        }
        return true;
       
    }
}



