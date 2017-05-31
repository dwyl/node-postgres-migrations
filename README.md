# node-postgres-migrations
Running migrations on node postgres

### Step 1
Copy over the migrations folder, callMigrations.js and migrations.js over to your project

### Step 2
Add the sql migrations you would like to run to the migrations folder (1 migration per file).
**The file names should start with the date in the format yy-mm-dd** (this is to ensure the migrations are run in the correct order - from top to bottom)

### Step 3
Add the environment variable DATABASE_URL

### Step 4
Run `node callMigrations.js`

If you want this to run on Heroku deployment, then add to your postinstall command in your package.json (it's probably a good idea to do this after you've taken a db backup!)
