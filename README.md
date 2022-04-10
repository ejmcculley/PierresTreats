# _PierresTreats_

#### By _**Erin McCulley**_

#### _Beginners Web Development_

## Technologies Used

* _C#_
* _ASP.NET Core_
* _Entity_
* _Identity_
* _MySQL Workbench_
* _Dotnet ef_
* _Razor_
* _Markdown_
* _Git / Github_
* _Terminal_

## Description

_Create a web application with authentication and authorization through Identity, two classes, and a many-to-many relationship. The user should have full CRUD functionality for Treats and Flavors, and be able to assign either class to the other._

## Setup/Installation Requirements

_To clone this repository:_

1. Click on the green "Code" button above this file list.
2. Copy the HTTPS link (this is the default option).
3. Open your local Terminal.
4. Navigate to the local directory where you want the cloned directory to go.
5. In your Terminal type "git clone" (without the quotes) then paste the URL you copied above. 
6. Press 'enter' and the cloned directory should be copied to your current working directory.

_To install C# and .NET:_

1. In your Terminal, navigate to HairSalon.Solution/HairSalon and type 'dotnet build' and 'dotnet watch run' to launch the web application.
2. Start by adding a new stylist, then you can fill out details for the stylist, and add clients to their roster. 

_To set up MySQL Workbench:_

1. Download and install MySQL Workbench [here](https://www.mysql.com/products/workbench/).
2. Create an appsettings.json file !!! Add this file to your .gitignore !!! by adding: */appsettings.json to your .gitignore file.
3. Add appsettings.json file in your main project directory. Enter the following into your appsettings.json file

{
    "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Port=3306;database=[YOUR-DATABASE-HERE];uid=root;pwd=[YOUR-PASSWORD-HERE];"
    }
}

_To Import Database_

1. In the Navigator -> Administration window, select Data Import / Restore
2. In Import Options, select Import from Self-Contained File
3. Navigate to file that was just created
4. Under Default Schema to be Imported To, select the New button
  - Enter the name of your database
  - Click OK
5. Go to Import Progress tab and click Start Import at the bottom right corner
6. Reopen  Navigator -> Schemas tab, right click and Refresh All

_To Set up Dotnet ef_

1. In your terminal type 'dotnet tool install --global dotnet-ef --version 5.0.1'
2. In the root directory of the project type 'dotnet add package Microsoft.EntityFrameworkCore.Design -v 5.0.0'
3. Next type 'dotnet ef migrations add Initial'
4. Then type 'dotnet ef database update' If everything worked correctly, you will have a database created for you!

_To Add Identity_

1. In your project's root directory type 'dotnet add package Microsoft.AspNetCore.Identity.EntityFrameworkCore -v 5.0.0'
2. Then run migrations by typing 'dotnet ef migrations add addIdentity' and 'dotnet ef database update'


## Known Bugs

* N/A

## License
MIT License

Copyright (c) [2021] [Erin McCulley]

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