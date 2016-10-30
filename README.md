import java.util.Scanner;
public class Count {


    public static void main(String[] args) throws Exception {


        java.io.File file = new java.io.File("C://file1.txt");

 

        Scanner input = new Scanner(file);

        String fileContent = "";


        while (input.hasNext()) {

            fileContent += input.next() + " ";

        }

     

        input.close();

        char[] charArr = fileContent.toCharArray();

        int counter = 0;

        for(char c : charArr)

        {

              if(c == 'a' || c == 'e' || c == 'i' || c == 'o' || c == 'u' || c == 'y')

                   counter++;

        }

        

        
        System.out.println("Number of Vowels: " + counter);

    }
}
