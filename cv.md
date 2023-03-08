# **Kirill Mezentsev**
## **Junior Full-stack Developer**
---
## **Contact information**

**E-mail:** <mezentsevkv91@gmail.com>   
**Discord:** [Kirill Mezentsev(@KirillVM)](OCB#1927)

## **About Myself**

Hi! My name is Kirill. I am a beginner web developer.
My purpose is to learn **JS(React, Angular) + C#** languages for having a new interesting(maybe not :D) job.
I learn something new about C# and JS every day and I like to do it!
I have been working as a production engineer in a big company about five years. We design cars.
When I was at university I realy liked programming, but i didn't understand how important it is for me.
But this year I said to myself: It's time for a change!

## **Skills**

* **Laguages**
   * JavaScript starter
   * C# basic (DI, SOLID, Multithreading, Collections, OOP)
   * Sql basic

* **Technologies**
   * .NET basic
   * .NET Core starter

* **Libraries**
   * LINQ basic
   * Entity Framework basic
   * jQuery

* **Database**
   * PostgreSQL starter
   * MySql starter

## **Code Example**

``` C#
class JsonStreamer<K>
{
    private static readonly JsonSerializerOptions options = new JsonSerializerOptions()
    {
        AllowTrailingCommas = true,
        PropertyNamingPolicy = JsonNamingPolicy.CamelCase,
        Encoder = JavaScriptEncoder.Create(UnicodeRanges.All),
        WriteIndented = true
    };
    public static void Write<T>(string path, K persons)
    {
        var write = WriterAsync<T>(path, persons);
    }
    public static K Read<T>(string path)
    {
        var read =  ReaderAsync<T>(path);
        return read.Result;
    }
    private static async Task WriterAsync<T>(string path, K persons)
    {
        System.Console.WriteLine("wr");
        using (FileStream fs = new FileStream(path, FileMode.OpenOrCreate, FileAccess.Write, FileShare.None))
        {
            await JsonSerializer.SerializeAsync(fs,persons,options);
        }
    }
    private static async Task<K> ReaderAsync<T>(string path)
    {
        System.Console.WriteLine("re");
        using (FileStream fs = new FileStream(path, FileMode.Open, FileAccess.Read, FileShare.Read))
        {
            return await JsonSerializer.DeserializeAsync<K>(fs, options);
        }
    }
}
```
## **Work Expiriens**

* Projects
   * [SerializationTask](https://github.com/KirillVM/SerializationTask.git) 
   * [ArtworkStore](https://github.com/KirillVM/ArtworkStore.git)   

## **Education**

**University:** Lobachevsky State University of Nizhny Novgorod   
**Faculty:** Faculty of Physics   
**Speciality:** Solid state electronics   

* **Courses:**
  * C# starter and basic (*ITVDN*)
  * Git (*ITVDN*)
  * ASP.NET Core statrer (*ITVDN*)
  * Python.Algorithms (*STEPIK*)
  * [Algorithms and data structures](https://www.youtube.com/watch?v=wFx6HAfJEnI&list=PLrS21S1jm43iUIpR51VCJgxY1MjwS-pAZ) (Pavel Marvin ITMO)

Jeffrey Richter awesome! :D

**English languege:** Elementary - Pre-Intermediate