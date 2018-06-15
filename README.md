# MySQL 
<a href="http://www.mysql.com/">MySQL</a> is a fast, multi-threaded,
multi-user SQL database server. IoMySQL is a MySQL binding for Io,
by <a href="http://dahlia.pe.kr/">Min-hee Hong</a>.

```Io
my := MySQL establish(&quot;localhost&quot;, &quot;user&quot;, &quot;password&quot;, &quot;database&quot;)

# Get rows by Map
my queryThenMap(&quot;SELECT * FROM rel&quot;) foreach(at(&quot;col&quot;) println)
# Get rows by List
my query(&quot;SELECT * FROM rel&quot;) foreach(at(0) println)

my close
```

# Installation
`MySQL` should be installed and foundable in your system. Then:

```
eerie installation https://github.com/IoLanguage/MySQL.git
```
