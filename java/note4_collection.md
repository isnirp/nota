
# Array, Collection and Maps
***
## array
- a collection of a fixed number of elements of the same type
  >`int[] arr = new int[2]{1,2};`
- Functions
    - arr.length *//a constant*
    - System.arraycopy(Object src, int srcPos,
      Object dest, int destPos, int length)
    - java.util.Arrays.stream(arr)... *//create stream from array*
    - java.util.Arrays.toString(arr) *//convert to string*

## collection
- store, retrieve, manipulate, and communicate aggregate data
- basic methods
    - int size()
    - boolean isEmpty()
    - boolean contains(e)
    - boolean add(e), remove(e)
    - iterator
- max operation methods
    - boolean addAll(c)
    - boolean removeAll(c)
    - boolean retainAll(c)
    - void clear()
- other
    - toArray()

### traversing collections
- aggregate operations
    - stream()
- for-each
- Iterator

## set
- collection that does not contain duplicate elements
- implementations
    - HashSet; stores elements in hashtable *//best impl*
    - TreeSet; orders elements based on their values
    - LinkedHashSet; impl as hashtable with linkedList. ordered by insertion
## list
- an ordered or sequence of collection
- may contain duplicates
- methods
    - positional access;
        - set(o), add(o), remove(o), addAll(c)
    - search;
        - indexOf(), lastIndexOf()
    - iteration;
        - listIterator(), listIterator(i)
            - hasNext(), next(), remove(), hasPrevious(), previous()
    - range;
        - fromIndex() toIndex()

## map

## generics
- java 1.5
- provides compile-time type safety to collections
- Example; List<String>, Collection<?>
- supertype for generics is the unknown type represented by the wildcard '?'
- generic methods:
    - allow type parameters to be used to express dependencies among the types of one or more arguments to a method and/or its return type.
    - where there's no dependency use the wildcards
    - >`static <T> void fromArrayToCollection(T[] a, Collection<T> c)`
