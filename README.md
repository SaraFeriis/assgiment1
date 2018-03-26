# assgiment1
bank part one
 public static void main(String[] args) {
        String input = JOptionPane.showInputDialog("Enter the amount:");
        
        // Convert the string to an integer and store it in the variable
        int amount = Integer.parseInt(input);
        
        // Print the converted integer value to the console using 
        System.out.println("Requested Amount=" + amount);
     
        // Declare the integer variables
        int  hundreds, fifties, twenties,tens, fives, twos,ones;
        
        // Declare another integer variable
        int remainingAmount;
        
        // Compute the numbers and the remainingAmount
        // and Print the information 
        hundreds = amount / 100;
        remainingAmount = amount - (hundreds*100);
        System.out.println("Hundreds = "+hundreds +", Remaining Amount = "+remainingAmount);
        
        fifties = remainingAmount / 50;
         remainingAmount = remainingAmount - (fifties*50);
        System.out.println("Fifties = "+fifties +", Remaining Amount = "+remainingAmount);
        
        twenties = remainingAmount / 20;
        remainingAmount = remainingAmount - (twenties * 20);
        System.out.println("Twenties = "+twenties +", Remaining Amount = "+remainingAmount);
        
        tens = remainingAmount / 10;
        remainingAmount = remainingAmount - (tens*10);
        System.out.println("Tens = "+tens +", Remaining Amount = "+remainingAmount);
        
        fives = remainingAmount / 5;
        remainingAmount = remainingAmount - (fives*5);
        System.out.println("Fives = "+fives +", Remaining Amount = "+remainingAmount);
       
        twos = remainingAmount / 2;
        remainingAmount = remainingAmount - (twos*2);
        System.out.println("Twos = "+twos +", Remaining Amount = "+remainingAmount);
        
        ones = remainingAmount;
        System.out.println("Ones = "+ones);
        
        //  show the summary of the value 
        JOptionPane.showMessageDialog(null,
        "Requested Amount (" + amount + ")\n" +
        "Hundreds (" + hundreds + ")\n" +
        "Fifties (" + fifties + ")\n" +
        "Twenties (" + twenties + ")\n" +
        "Tens (" + tens + ")\n" +
        "Fives (" + fives + ")\n" +
        "Twos (" + twos + ")\n" +
        "Ones (" + ones + ")" );
 
     
    
    }
    
}
