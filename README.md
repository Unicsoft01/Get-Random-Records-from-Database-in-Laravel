# Get-Random-Records-from-Database-in-Laravel

In the project development sometimes we need to display random data on Frontend that time we need to fetch random records from the database to display random records on the frontend. In Laravel, There are some methods to get random records from the database.

This article will teach you how to get random records from the database.

## works for Laravel >= 5.2


```Post::select('id', 'title' ,'slug')->inRandomOrder()->get();```

Also, If you want to get limited random records then you can use this method to get limited random records.

```// Random Record with a limit```
```Post::select('id', 'title' ,'slug')->inRandomOrder()->limit(10)->get();```

```// Single Random Record```
```Post::select('id', 'title' ,'slug')->inRandomOrder()->first();```
