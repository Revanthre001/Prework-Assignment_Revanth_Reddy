# Prework-Assignment_Revanth_Reddy
import java.util.Scanner;

class FirstLetterPrinter {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        String input = in.nextLine();
        System.out.println(firstLetterPrinter(input));
    }
    static String firstLetterPrinter(String str){
        String output = new String("");
        if(str.length()==0){
            return "nostrfound";
        }
        output = output+str.charAt(0);
        for(int i = 1; i< str.length();i++){
            if (str.charAt(i) == ' '){
                output+=str.charAt(i+1);
            }
        }
        return output;
    }
}
