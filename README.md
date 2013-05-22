deck
====
public class Deck extends Card
{
   private ArrayList<Card> deck;
  

public static int values = 13; 
public static int suits = 4; 
public static int aCard =values * suits; 

Card[] deck = new Card[aCard -1]; 
int x = 0; 

public Deck()
 {
while(x < 52)
{ 


for(int i = 1; i <= values; i++)
    {

    for(int y = 1; y <= suits; y++)
        {

        deck[x] = new Card(i,y); 
        x++; 
        }
    }

}
}

    public Card getCard(int p)
    {
    return deck[p-1];   
    }
}
