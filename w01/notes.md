[README.md](../README.md)

## Week 01

### 1. Web API with ASP.NET Core controllers (`ContosoPizza`)

Built from the *Create a web API with ASP.NET Core controllers* module.

**Project:** [w01/ContosoPizza/](w01/ContosoPizza/)

**CRUD Implemented**: `GET /pizza`, `GET /pizza/{id}`, `POST /pizza`, `PUT /pizza/{id}`, `DELETE /pizza/{id}`.

**Evidence** : [Image](./ContosoPizza/crud-working.jpg)

### 2. Sales summary function (Part 2)

`CalculateSalesTotal` from [w01/mslearn-dotnet-files/Program.cs](w01/mslearn-dotnet-files/Program.cs):

````csharp
double CalculateSalesTotal(IEnumerable<string> salesFiles)
{
    double salesTotal = 0;

    // Loop over each file path in salesFiles
    foreach (var file in salesFiles)
    {
        // Read the contents of the file
        string salesJson = File.ReadAllText(file);

        // Parse the contents as JSON
        SalesData? data = JsonConvert.DeserializeObject<SalesData?>(salesJson);

        // Add the amount found in the Total field to the salesTotal variable
        salesTotal += data?.Total ?? 0;
    }

    return salesTotal;
}
````