public class Main {
static boolean isPalindrome(int number){
    int temp = number, reverseNumber=0 ,lastNumbers;
    while(temp!=0){
        lastNumbers=temp%10;
        reverseNumber=(reverseNumber*10)+lastNumbers;
        temp/=10;
    }
    if(reverseNumber==number)
        return true;
    else
        return false;



}
    public static void main(String[] args) {
        System.out.println(isPalindrome(10));
    }
}
