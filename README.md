# Bubble-Sorting-Java
Bubble Sorting Java
public class bubblesorting {
    
    public static void bubbleSort(int[] arr) {
        int n = arr.length;
        for(int i = 0; i < n - 1; i++) {
            for(int j = 0; j < n - i - 1; j++) {
                if(arr[j] > arr[j + 1]) {
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }

    public static void main(String[] args) {
        int[] arr = {64, 45, 23, 12, 55, 78, 89};
        bubbleSort(arr);
        System.out.println("Sorted array:");
        for(int num : arr) {
            System.out.println(num);
        }
    }
}
# check the output of bubble sorting 
12
23
45
55
64
78
89
