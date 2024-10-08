# Day 2 Workshop

## Reading transactions

The support team keep their records in CSV format. Their records for 2014 are
stored in `data/Transactions2014.csv`

Note that there’s a header row, telling you what each column means. Every record
has a date and represents a payment from one person to another person. There’s
also a narrative field which describes what the payment was for.

The person in the ‘From’ column is paying money, so the amount needs to be
deducted from their account. The person in the ‘To’ column is being paid, so the
amount needs to be added to their account.

Use a class for each type of object you want to create.

You should add two commands:

- [ ] `supportbank transaction summarise` – should output the names of each
      person, and their current balance according to `Transactions2014.csv`.

- [ ] `supportbank transaction list <account name>` – should print a list of
      every transaction, with the date and narrative, for that person’s account.
      For example, `supportbank transaction list "jon a"` would list all of Jon
      A’s transactions.

## Moving on

Once you have dealt with `data/Transactions2014.csv`, there are some other files
in the `data` folder - see if you can make the application work with those, too.
You might need to do some research online to see how to deal with issues that
may crop up.

## Hints

### Working with csv

There is a note on
[working with CSV](https://tech-docs.corndel.com/java/file-io.html#csv) which
will give you some ideas about using split and join to deal with rows of CSV.

### Removing the CSV header

There are a number of ways we could remove the header row from the CSV.
[`.remove(0)`](https://tech-docs.corndel.com/java/lists.html#arraylist-methods)
or
[`.sublist()`](https://tech-docs.corndel.com/java/list-techniques.html#sublists)
could be used.

### JSON lists

There is a note on
[parsing lists of JSON](https://tech-docs.corndel.com/java/working-with-json.html#json-lists)
which will help with `2013.json`.

### XML

There are notes on how to parse XML
[here](https://www.baeldung.com/java-xerces-dom-parsing)
