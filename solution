class Solution {
    public static String countAndSay(int n) {
        if (n <= 0) {
            return "";
        }
        
        String result = "1";
        
        for (int i = 1; i < n; i++) {
            result = getNextSequence(result);
        }
        
        return result;
    }
    
    private static String getNextSequence(String current) {
        StringBuilder nextSequence = new StringBuilder();
        
        int count = 1;
        char digit = current.charAt(0);
        
        for (int i = 1; i < current.length(); i++) {
            if (current.charAt(i) == digit) {
                count++;
            } else {
                nextSequence.append(count).append(digit);
                digit = current.charAt(i);
                count = 1;
            }
        }
        
        nextSequence.append(count).append(digit);
        
        return nextSequence.toString();
    }
}
