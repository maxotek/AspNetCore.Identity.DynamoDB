# AspNetCore.Identity.DynamoDB
[![Travis Build Status](https://travis-ci.org/miltador/AspNetCore.Identity.DynamoDB.svg?branch=master)](https://travis-ci.org/miltador/AspNetCore.Identity.DynamoDB)
[![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/ooa12u8cdp3t0nss?svg=true)](https://ci.appveyor.com/project/miltador/aspnetcore-identity-dynamodb)
[![NuGet package version](https://img.shields.io/nuget/v/AspNetCore.Identity.DynamoDB.svg)](https://www.nuget.org/packages/AspNetCore.Identity.DynamoDB)

[DynamoDB](https://aws.amazon.com/dynamodb/) data store adaptor for [ASP.NET Core Identity](https://github.com/aspnet/Identity),
which allows you to build ASP.NET Core web applications, including membership, login, and user data.With this library,
you can store your user's membership related data on DynamoDB.

## Using the Library

[The library is available at NuGet.org](https://www.nuget.org/packages/AspNetCore.Identity.DynamoDB).
You can start using the library by integrating it into your `project.json` file.
This library supports [`netstandard1.6`](https://docs.microsoft.com/en-us/dotnet/articles/standard/library).

### Samples

You can find some samples under [./samples](./samples) folder and each of the sample contain a README file
on its own with the instructions showing how to run them.

### Tests

In order to be able to run the tests, you need to have DynamoDB up and running on `localhost:8000`.
You can easily do this by running the below Docker command:

```bash
docker run -p 8000:8000 dwmkerr/dynamodb -sharedDb -inMemory
```

After that, you can run the tests through your preferred test runner (e.g. JetBrains Rider test runner)
or by invoking the `dotnet test` command under the test project directory.

## Notes

The project is based on awesome work of @tugberkugurlu who created [MongoDB](https://github.com/tugberkugurlu/AspNetCore.Identity.MongoDB) 
adaptor to AspNetCore, rewritten and adapted to the specifics of DynamoDB.

## License

The MIT License (MIT)

Copyright (c) 2016 Tugberk Ugurlu
<br/>
Copyright (c) 2017 Vasiliy Solovey

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
