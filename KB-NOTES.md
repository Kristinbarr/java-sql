#### Setting up for this project
- install Postgres
- install pgAdmin4, open in browser
- clone/copy sql to local


__inside pgAdmin4:__
- pgAdmin is good for viewing and making slight changes
- creating db is not done pgAdmin
- writing DML is done in Spring

__Create new Postgres DB:__
- on server, right click -> 'Create' -> 'Server'
  - you can have mulitple servers
  - General Settings tab: name server
    - ex: 'My local PG server'
    - this will show as a new DB in Postgres
  - Connection tab: set Host name/address to 'localhost'
    - leave port at 5432 (default)
    - Username is Postgres user/pass
      - try 'password'
      - environment variables are set with user/pass?
  - Save
- Schemas:
  - usually have multiple schemas
  - multiple copies of the db to test and experiement
  - when testing/developing, don't affect production

__Create a DB:__
- on 'Database', right click -> 'create' -> 'create db'
  - General settings: set Database name (ex: 'Northwind2')

__Add to DB/create table:__
- 'Tools' -> 'Query Tool'
- most of the queries are done here
- click 'open folder icon'
- select sql document
  - this brings in DML (data manipulation lang)
- execute by clicking top center lighting bolt icon
- refresh table list
  - right click -> 'refresh'
  - tables should appear

__view a single table:__
- tables are also called entities
- right click on any table -> 'view and edit data' -> 'all rows'
  - in our Java world:
    - table is our class
    - columns are our class fields
    - rows are individual objects for the class
  - ability to change data in db at this point

__SQL__
- open new query editor, clear previous query
  - 'Tools' -> 'Query tool'
- make query
- to run, click upper right/center lightning bolt icon
