# RPS-game
// A computer and user game

import java.util.Scanner;
import java.util.Random;
public class RPS_game {
    public static void main(String[] args) {
        System.out.println("1=rock\n2=paper\n3=scissor");
        Scanner sc =new Scanner(System.in);
        int userInput = sc.nextInt();
        Random random= new Random();
        int computerInput =random.nextInt(3);
        if (userInput==computerInput){
            System.out.println("draw");
            }
        else if (userInput==0&&computerInput==2 || userInput==1&&computerInput==0 ||userInput==2&&computerInput==1)
        {
            System.out.println("you won");
        }
        else {
            System.out.println("you loss");
        }

    }
}

