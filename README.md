# Height-Checker-using-Java-Leetcode

    class Solution {
        public int heightChecker(int[] heights) {
            int arr[] = new int[heights.length];
            int result =0;
            for(int i =0; i<heights.length;i++){
                arr[i] = heights[i];
            }
            Arrays.sort(heights);
            for(int i =0; i<heights.length;i++){
                if(arr[i]!=heights[i]){
                    result++;
                }
            }
            return result;
        }
    }
