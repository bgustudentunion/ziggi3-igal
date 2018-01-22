# Ziggi 3.0

## Installation

Ziggi 3.0 is a nodejs application. Install the prerequisites below and a simple:

```
git clone https://github.com/igalshapira/ziggi3.git
cd ziggi3
npm install
npm start
```

should do the work.

## Prerequisites

* Install [nodejs](https://nodejs.org/en/download/)
* Choose database. You can use one of the two:
  * Download and install [mongodb](https://www.mongodb.com/)\
    * Set environment variable: set MONGO_CONNECTION_STRING=mongodb://localhost/ziggi
  * Use [Azure CosmosDB](https://azure.microsoft.com/en-us/try/cosmosdb/)
    * Set API to MongoDB
    * Set environment variable: set MONGO_CONNECTION_STRING=mongodb://{yourdb}:{yourkey}@{yourdb}.documents.azure.com:10255/?ssl=true


## History

Ziggi 1 was started at 2006, based on [LAMP](https://en.wikipedia.org/wiki/LAMP_(software_bundle)) architecture. The code was originally published in google code.
The source code is no longer available.

Ziggi 2 project was based on Ruby On Rails, using postgres database. The source code was never published. The site went on air in 2013 and it is the current running ziggi version (http://www.ziggi.co)

Ziggi 3 is a new project, based on MEAN stack. With no actual plans of when and where and if to deploy it.

## Migrations

Create a new migration

```
node_modules\.bin\migrate create <migration-name>
```

Run migrations

```
npm install
```

## API

Api documentation can be generated using [Apidoc](http://apidocjs.com/).

```
grunt apidoc
```

## Hebrew Holidays

Hebrew holidays are based on [HebCal Jewish calendar REST API](https://www.hebcal.com/home/195/jewish-calendar-rest-api).

Each year holidays are loaded and stored in the data base using `grunt hebcal <--year=year>`

## License

Ziggi3 is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or
(at your option) any later version.

Ziggi3 is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

See full license in LICENSE file.