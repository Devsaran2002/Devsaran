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
