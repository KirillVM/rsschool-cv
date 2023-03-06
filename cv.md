# **Kirill Mezentsev***
---
## __Contacts__

email:[mezentsevkv91@gmail.com][mezentsevkv91@gmail.com] 
discord:[Kirill Mezentsev(@KirillVM)][OCB#1927]

## __ABOUT ME__

Hi!My name is Kirill. I am a beginner web developer.
My purpose is to learn JS(React, Angular) + C# languages for having a new interesting(maybe not :D) job.
I learn something new about C# and JS every day and I like it!
I have worked as a production engineer in a big company over five years. We made cars.
When I was at university I realy liked programming, but i didn't understand how important it was.
But this year I said to myself: It's time to change!

## __Skils__

* Laguages
   * C# basic (DI, SOLID, Multithreading, Collections, OOP)
   * Sql basic
   * JavaScript starter

* Technologies
   * .NET basic
   * .NET Core starter

* Technologies
   * LINQ basic
   * Entity Framework basic

* Database
   * PostgreSQL
   * MySql

## __Code Examples__

'''C#
    class JsonStreamer
    {
        private static readonly JsonSerializerOptions options = new JsonSerializerOptions()
        {
            AllowTrailingCommas = true,
            PropertyNamingPolicy = JsonNamingPolicy.CamelCase,
            Encoder = JavaScriptEncoder.Create(UnicodeRanges.All),
            WriteIndented = true
        };
        public static void Write<T>(string path, Person[] persons)
        {
            var write = WriterAsync<T>(path, persons);
        }
        public static Person[] Read<T>(string path)
        {
            var read = ReaderAsync<T>(path);
            return read.Result;
        }
        private static async Task WriterAsync<T>(string path, Person[] persons)
        {
            using (FileStream fs = new FileStream(path, FileMode.OpenOrCreate, FileAccess.Write, FileShare.Read))
            {
                await JsonSerializer.SerializeAsync(fs,persons,options);
            }
        }
        private static async Task<Person[]> ReaderAsync<T>(string path)
        {
            using (FileStream fs = new FileStream(path, FileMode.Open, FileAccess.Read, FileShare.Write))
            {
                return await JsonSerializer.DeserializeAsync<Person[]>(fs, options);
            }
        }
    }
'''
## __Work Expiriens__

* Projects
   * [SerializationTask][https://github.com/KirillVM/SerializationTask.git] Working with JSON files. Asynchronous write and read.
   * [ArtworkStore][https://github.com/KirillVM/ArtworkStore.git] Working with linq и EF. Using pattern MVC.

## __Education__

University: Lobachevsky State University of Nizhny Novgorod
Faculty: Faculty of Physics
Speciality: Solid state electronics

* Courses:
  * C# Starter and Basic *ITVDN*
  * Git *ITVDN*
  * Python.Algorithms. *STEPIK*

Jeffrey Richter awesome! :D

__English languege:__
Elementary - Pre-Intermediate