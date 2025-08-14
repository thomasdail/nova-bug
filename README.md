Seed the db:
```bash
$ php artisan migrate:fresh --seed
```

Login as the `test@example.com` user

Open the `Posts` resource
- You will see both the actions and edit buttons are missing

Open `app/Nova/Post.php`
- Move the `HasMany` field to anywhere other than the first entry in the array
- Both the actions and edit buttons now show
