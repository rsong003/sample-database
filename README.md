# Sample database

## Import database

### 1. Clone repository

1. Create a new directory on your localhost
2. Clone GitHub repository using either SSH or HTTPS URL:

Use HTTPS URL: `git clone https://github.com/michaljuhas/sample-database.git`

or alternatively the SSH URL: `git clone git@github.com:michaljuhas/sample-database.git`

You can read more about [Which remote URL should I use?](https://help.github.com/articles/which-remote-url-should-i-use/).

### 2. Unzip SQL files

Go to a sub-folder - either `/MySQL/` and decompress all `.tar.gz` files:

First, extract the first file:

`tar -xzf sample_ip.tar.gz`

Then merge 3 files into one and then extract

```
cat sample_staff_* > sample_staff.tar.gz
tar -xzf sample_staff.tar.gz
```

### 3. Load to your local database

Load the data to your local MySQL database

```
mysql -u root sample_ip < sample_ip.sql
mysql -u root sample_staff < sample_staff.sql
```

And you're done! Enjoy and check my course on Udemy:

* [Practice advanced SQL with MySQL](https://www.udemy.com/practice-advanced-sql-with-mysql/)
