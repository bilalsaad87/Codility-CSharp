using System;
using System.Collections.Generic;
using System.Linq;
// you can also use other imports, for example:
// using System.Collections.Generic;

// you can write to stdout for debugging purposes, e.g.
// Console.WriteLine("this is a debug message");

class Solution {
    public int solution(int[] A) {
        // write your code in C# 6.0 with .NET 4.5 (Mono)
        // The Main Idea to us dictionary < key, Value > pair to store every key with 
        // Occurrences value.
        Dictionary<int, int> occurrencesDic = new Dictionary<int, int>();

        for(int i =0; i< A.Length; i++)
        {
            if (occurrencesDic.ContainsKey(A[i]))
            {
                int occurrences =  occurrencesDic[A[i]];
                occurrences++;
                occurrencesDic[A[i]] = occurrences;
            }
            else
            {
                occurrencesDic[A[i]] = 1;
            }
        }

        int[] Keyset = occurrencesDic.Keys.ToArray();

        foreach(int currentkey in Keyset)
        {
            int occurrences = occurrencesDic[currentkey];

            if(occurrences % 2 != 0)
            {
                return currentkey;
            }
        }

        return 0;
    }
}
