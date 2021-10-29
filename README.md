## First-time deployment

After running the docker-compose.yml,

run the following commands on the vegestats image:

```
rake db:create
rake db:migrate
```

This will create the database for the web app.

The database is repopulated whenever the vegebot image is first run, so after runnning this command it is required to restart this image.

If future changes to the tables in the database are required, the migration command will have to be repeated.