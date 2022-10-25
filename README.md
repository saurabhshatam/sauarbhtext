# sauarbhtext you can add
solved :: - >
public class GFG_6 {
    //revers the array
    public static void main(String[] args) {
        int arr[] = {1,2,3,4,5,6};
        printArray(arr,6);
        reverseArray(arr,0,5);
        System.out.println("Reversed array is \n");
        printArray(arr, 6);
    }
    static void printArray(int arr[], int size){
        for (int i = 0; i < size; i++) {
            System.out.printf(arr[i] + " ");
        }
    }
    static void reverseArray(int[] arr, int start , int end){
        int temp;

        while (start<end){
            temp = arr[start];
            arr[start] = arr[end];
            arr[end] = temp;
            start++;
            end--;
        }
    }
}
