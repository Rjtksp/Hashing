# Hashing
Introduction to Hashing.

## HASHMAP:
HashMap<K, V> is a part of Java’s collection since Java 1.2. This class is found in java.util package. It provides the basic implementation of the Map interface of Java. It stores the data in (Key, Value) pairs, and you can access them by an index of another type (e.g. an Integer). One object is used as a key (index) to another object (value). If you try to insert the duplicate key, it will replace the element of the corresponding key.

## Syntax:
HashMap<Character, Integer> map = new HashMap<>();

### Methods:
map.containsKey();
map.put(x,y);
map.get(x);
map.getKey();
map.getValue();
map.keySet();
map.values();
map.size();
map.remove();

## ABCABA to A 3 B 2 C 1 ?
```js
import java.util.HashMap;
public static void main(String[] args) {
        String str = "ABCABA";
        char[] arr = str.toCharArray();
        HashMap<Character, Integer> map = new HashMap<>();
        
        // filling data in map
        for(int i=0; i<arr.length; i++){
            if(map.containsKey(arr[i])){
                map.put(arr[i], map.get(arr[i]) + 1);
            }else{
                map.put(arr[i], 1);
            }
        }
        
        // Printing key:values pair
        for(Map.Entry<Character, Integer> ite : map.entrySet()){
            System.out.print(ite.getKey() + "-" + ite.getValue() + " ");
        }
    }
```

