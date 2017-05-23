package pigLatin;
import javax.swing.*;// importing package in order to use JOptionPane.
public class pigLatin2 {
    public static void main(String[] args) { //main method
        String userSen;//--declaring a string variable (userSen) for the users input
        
//*****************************************************************************************************************
           userSen=JOptionPane.showInputDialog(null,"Enter your words here: ", "PIG LATIN", JOptionPane.INFORMATION_MESSAGE);//assigning String(userSen) by asking user for input
       
if (userSen.isEmpty()){//if user does not input a word program will stop and tell user to input a word
JOptionPane.showMessageDialog(null,"PLEASE ENTER IN A WORD", "PIG LATIN", JOptionPane.INFORMATION_MESSAGE);
}         
//*****************************************************************************************************************
else{//if user does input a word
            for (int i= 0; i < 1;i++){ //for statement 
                if (userSen.startsWith("a") || userSen.startsWith("e") || userSen.startsWith("i") || userSen.startsWith("o") || userSen.startsWith("u"))//if word user enters starts with a vowel....
                    JOptionPane.showMessageDialog(null,userSen+ "way ", "PIG LATIN", JOptionPane.INFORMATION_MESSAGE);//print out word + way
                else //Or...
                    if (userSen.startsWith("sh") || userSen.startsWith("ch") || userSen.startsWith("th")) // if word starts with a consonant ...
                    JOptionPane.showMessageDialog(null,userSen.substring(2)+userSen.substring(0,2)+"ay ", "PIG LATIN", JOptionPane.INFORMATION_MESSAGE);//Substring method-print out third letter of word + first and third letter of word + "ay" (0 counts in java)
                else//if word does not start with a vowel or consonant...
                    JOptionPane.showMessageDialog(null,userSen.substring(1)+userSen.substring(0,1)+"ay ", "PIG LATIN", JOptionPane.INFORMATION_MESSAGE);//print out secound letter of word + first and secound letter + "Ay"
}
}
} 
}
//*****************************************************************************************************************

//END OF PROGRAM..
