## Lab06 Task 01
    In this directory, you will find a file called csv/contacts.csv. Use regular expressions to extract the following information from it.
    Remember that you can use different tools like grep, awk, or sed to use regular expressions from the command line. Pipes might also be helpful.
    Document your commands and the corresponding outputs with verbatim formatting in a Markdown file called parse_contacts.md. Alternatively, you can write a bash script parse_contacts.sh with all commands.
--- 

1. Extract all email addresses from the text.
2. Extract all phone numbers from the text.
3. Extract all names that start with the letter ‘J’.
4. Extract all street names that contain the word 'St'.
5. Extract the last names of all people.
6. Extract all email domains (part after the @ sign).
7. Find all entries where the phone number ends with ‘7’.
8. Extract all instances of first names that end with the letter 'e'.

## Answers
```bash

1. grep -Eo "[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}" contacts.csv
2. grep -Eo "\([0-9]{3}\) [0-9]{3}-[0-9]{4}|1-[0-9]{3}-[0-9]{3}-[0-9]{4}" contacts.csv
3. grep -Eo "J[A-Za-z]* [A-Za-z'-]+" contacts.csv
4. grep -Eo "\w+\sSt\.?" contacts.csv
5. awk -F',' '{print $1}' contacts.csv | awk '{print $NF}'
6. grep -Eo "@[A-Za-z0-9.-]+\.[A-Za-z]{2,}" contacts.csv | sed 's/@//'
7. grep -E "7$" contacts.csv
8. grep -Eo "[A-Za-z]*e [A-Za-z'-]+" contacts.csv

```
