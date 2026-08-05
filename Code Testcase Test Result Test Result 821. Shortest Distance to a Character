class Solution {
    public int[] shortestToChar(String s, char c) {
        int n = s.length();
        int[] ar = new int[n];
        int i = 0, j = 0;
        int temp = Integer.MAX_VALUE;

        while (j < n) {
            if (s.charAt(j) == c) {
                while (i <= j) {
                    ar[i] = Math.min(Math.abs(j - i), Math.abs(temp - i));
                    i++;
                }
                temp = j;
            }
            j++;
        }
        while (i < n) {
            ar[i] = Math.abs(temp - i);
            i++;
        }

        return ar;
    }
}
