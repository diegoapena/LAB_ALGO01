# LAB_ALGO01


EJERCICIO 1
int SumScores (int[]scores)
 {
    // (+1(asignacion))
     int sum = 0;

   (+1(init)) + (N+1(comparacion)) + (N (incremento))
    for (int i= 0 ; i < scores.length; i++)
    {
       //(1(incremento)) (1(asignamiento)) + (N (indice))
        sum += scores[i]
     }
      //  +1
      return sum;
}

1 + 1 + (n+1) + n + 2  + N+ 1 
T(N)=3n + 6
O(N) = N

--------------------------------------------------------------------
EJERCICIO 2


void ComparePlayers(List<GameObject> players)
{
//  (+1(int)) +   (n+1 (comparaciones)) + (n (incrementos))  
   for (int i = 0 ; i < players.Count; i ++ )
   {  
       //   (+1(init))  + (n+1 (comparacion)) + (n(incrementos))  
      for ( int j = i + 1; j < players.Count; j++)
      {
        // ( (+1(operacion)) + (n(asignacion))  +  (1(suma) +  (1(suma)    
          Debug.Log( players[i].name + "vs" + ----------------);
      }
   }
}
 FOR interno:
 
 (4N + 6)
 (4N + 6)*N
 4N² +6N
 
 FOR externo:
 4N² +6N + 2N + 2
4N² + 8N + 2
 T(N) = 4N² + 8N + 2
 O(N) = N² 

------------------------------------------------------------------------

 EJERCICIO 3 :
 
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
          //   (1(asignacion))  + (1(ncremento)) + (N)
             int interaction = players[i] + players[j];
             //  (1(incremento)) + (1(asignacion))
             score += interaciction;
          }
    }
     // (+ 1)
     return score;
 }

 FOR Interno:
 3N + 2N + 2N + 3
 (5N + 7) * N
 5N² + 7N
 for Externo:
  2N + 2
  2N + 2 + 5N² + 7N + 1 
  5N² + 9N + 3
  T(N) = 5N² + 9N + 3
  O(N) = N²
  

---------------------------------------------------------------------------------------
  EJERCICIO 4 :
  int CalculateFinalDamge ( int attack , int defense , float multiplier)
  {
    // (1(asignacion)) + (1 (resta))
     int baseDamage = attack - defense;
     // (asignacion))  + (1 multiplicacion))
     int finalDamage = (int)(baseDamage * multiplier);
          // (1(comparacion))
          if (finalDamge < 0)
          {
             // (1(asignacion))
              finalDamage = 0;
          }
          // (1)
          return finalDamage;
  }

  7
  T(N) = 7
  O(N) = 1
  
-------------------------------------------------------------------------------------------------
  
  EJERCICIO 5:
  
bool CanCastSpell(int mana , int cost)
{
      (1(asignamiento) + (1 (resta))
     int remainingMana = mana - cost;
     (1(comparacion))  + (1( asignamiento))
   if(remainingMana >= 0)
    {
      (1)
       Debug.Log("Spell casted");
       //(1) 
       return true;
     }
 // (1)
  return false;
}

7
T(N) = 7
O(N) = 1

------------------------------------------------------------------------------------------------

EJERCICIO 6:

Bool HasLowHealthPlayer(int[] healhValues)
 {
    (1(signamiento)) + (N+1(comparacion)) + (N(incremento))
    for(int i = 0 ; i <healthValues.Length; i ++1)
     {
      (1(asignamiento) + (N(indice))
       int health = healthValues.Length[i];
       (1(comparacion))
      if(health < 30)
        {
            (1)
           Debug.Log("Low health detected")
            (1)
            return true;
        }
        (1)
       return false;
      }
}

T(N)=3N + 7
O(N)= N

---------------------------------------------------------------------------------------------

EJERCICIO 7 :

int CountStrogerPairs(int[] powerLevels)
 {
    +1 asignamiento
     int count = 0;
     +1 asignamiento + (N+1) comparacion + N incremento
     for(int i = 0; i< powerLevels.Length; i++)
     {
       +1 asignamiento + (N+1) comparacion + N incremento
        for(int j = 0; j< powerLevels.Length;j++)
        {
           +N indice + 1 comparacion + N indice
          if(powerLevels[i] > powerLevels[j])
          {
            +1 por ejecucion -> +N por cada ejecucion completa del for interno
            count++;
          }
        }
     }
}

FOR interno:
(5N + 4)N
5N² + 4N

FOR externo:

5N² + 4N + 2N + 2
5N² + 6N + 2


T(N) = 5N² + 6N + 2
O(N) = N²
  

  
     

 
 

 
