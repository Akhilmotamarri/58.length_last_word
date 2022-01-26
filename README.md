# 58.length_last_word
java
class Solution {
    public int lengthOfLastWord(String s) {
        
        int n=s.length(),c=0;
        while(n>0)
        {
            if(s.charAt(--n)!=' ') c++;
            else if(c>0) return c;
        }
        return c;
    }
}
