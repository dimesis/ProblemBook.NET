# «ExceptionYieldYield» (Задача)
В какой момент произойдёт `Exception`?
```cs
public static IEnumerable<int> GetSmallNumbers()
{
  throw new Exception();
  yield return 1;
  yield return 2;
}
void Main()
{
  var numbers = GetSmallNumbers();
  var evenNumbers = numbers.Select(n => n * 2);
  Console.WriteLine(evenNumbers.FirstOrDefault());
}
```
[Решение](./ExceptionYieldYield-A.md)
