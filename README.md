deck
====
import java.util.ArrayList;

public class Deck
{
   private ArrayList<Card> deck;
  

public static int values = 13; 
public static int suits = 4; 
public static int aCard =values * suits; 



public Deck()
 {
     int x = 0;
while(x < 51)
{ 

    for(int y = 1; y <= suits; y++)
        {

        deck[x] = new Card(y,"HEARTS"); 
        x++; 
        }
    for(int j = 1; j <= suits; j++)
    {
        deck[x] = new Card(j, "SPADES");
        x++;
    }
    for(int u = 0; u <= suits; u++)
    {
        deck[x] = new Card(u, "DIAMONDS");
        x++;
    }
    for(int q = 0; q <= suits; q++)
    {
        deck[x] = new Card(q, "CLUBS");
        x++;
    }
    
}
}

public Card getCard(int p)
    {
    return deck[p-1];   
    }
}
