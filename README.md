//Reverse Str
import java.util.*;
public class reverse_str {
    public static void main(String args[]){
        Scanner scan = new Scanner(System.in);
        System.out.println("Enter the string ");
        String a=scan.nextLine();
        char arr[]=a.toCharArray();
        
        int left = 0;
        int right = arr.length-1;
        char temp='0';

        while(left<right){
            temp = arr[left];
            arr[left]=arr[right];
            arr[right]=temp;
            right--;
            left++;
        }
        System.out.println(arr);
        System.out.println(Arrays.toString(arr));
    }
}

//Prime number
public class prime {

    static boolean isPrime(int n) {

        if(n<=1){
            return false;
        }

        for(int i = 2;i<n;i++){
            if(n%i == 0){
                return false;
                
            }
        }
        return true;
    }
    public static void main(String args[]){
        int n = 9;
        
        if(isPrime(n)){
            System.out.println("true");
        }
        else{
            System.out.println("false");
        }
    }
}


// Factorial 

import java.util.*;
public class factorial {

    public static int factorial(int n){
        int res = 1;
        for(int i=2;i<=n;i++){
            res = res*i;
        }
        return res;
    }
    public static void main(String[] args){
        int num = 6;

        System.out.println(factorial(num));
    }
}

