# Recursion-Subsequence-of-string-




class Subsequence{
    static void Subseq(String s, String ans){
        if(s.length()==0){
            System.out.println(ans);
            return;
        }
        //pick case
        Subseq(s.substring(1),ans+s.charAt(0));
        //not pick case
        Subseq(s.substring(1), ans);
    }
    public static void main(String... args){
        System.out.println("Enter the String... ");
        Scanner str=new Scanner(System.in);
        String s=str.next();
        Subseq(s," ");


    }
}






/*
Enter the String...
do
 do
 d
 o

 */
