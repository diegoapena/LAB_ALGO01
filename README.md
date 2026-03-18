# LAB_ALGO01

----------------------------------------------------------------------
EJERCICIO 1


void ComparePlayers(List<GameObject> players)
{
//  (+1(int)) +   (n+1 (comparaciones)) + (n (incrementos))  = 2N+2
   for (int i = 0 ; i < players.Count; i ++ )
   {  
       //   (+1(init))  + (n+1 (comparacion)) + (n(incrementos)) = 2N+2
      for ( int j = i + 1; j < players.Count; j++)
      {
        // ( (+1(operacion)) + (n(asignacion))  +  (1(suma) +  (1(suma) =N+3    
          Debug.Log( players[i].name + "vs" + ----------------);
      }
   }
}
 FOR interno:
 2N+2 + N+3 = N(3N+5) 
 3N² + 5N
 FOR externo:
 3N² + 5N + 1 + N+1 + N 
 3N²+ 7N + 2

 T(O)=

------------------------------------------------------------------------

 EJERCICIO 2 :
 
 int CalculateInterractionScore(int[] players)
 {  
    // (1(asignacion)) 
     int score = 0;
     //  (1(init)) + (n+1( comparaciones)) + (n(incrementos))
     for( int i = 0; i < players.Length; i ++)
     {
      //   ( (1(init))  +   (n+1(comparaciones)) + (n(incrementos))
         for ( int j = i + 1 ; j < players.Lenght; j++)
          {
          //   (1(asignacion))  + (1(acceso)) + (1(acceso))
             int interaction = players[i] + players[j];
             //  (1(suma))
             score += interaciction;
          }
    }
     // (+ 1)
     return score;
 }

 FOR Interno:
 

---------------------------------------------------------------------------------------
  EJERCICIO 3 :

  int CalculateFinalDamge ( int attack , int defense , float multiplier)
  {
     int baseDamage = attack - defense;
     int finalDamage = (int)(baseDamage * multiplier);
          if (finalDamge < 0)
          {
              finalDamage = 0;
          }
          return finalDamage;
  }
  

  
     

 
 

 
