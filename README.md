# miquel-montoro-pilotes-challenge
| Developer      |    Date    | Version |
|:---------------|:----------:| ------: |
| Daniel Pedroza | 2024/06/27 |   1.0   |

## Summary

Create a Spring based application that allows us to manage the orders of the "pilotes" through some API. Pilotes of the great Miquel Montoro are a Majorcan recipe that consisting of a meatball stew.

The following operations must be implemented: 
- Create a pilotes order, choosing between 5, 10 or 15 pilotes.
- Update a pilotes order. During the 5 minutes following the creation of the order it will be allowed to update the order data; after that time it will not be possible to modify any data of the order because Miquel will be occupied cooking thepilotes.
- Search orders by customer data. Allow partial searches: e.g., all orders of customers whose name contains an “a” in their name.

All types of data used must be validated. For example, if you use an email when placing the order, you must validate that the format of the email is valid.

The search operation must be secured, you must check that the user is allowed to use the search. All other operations are public and should not be secured.



## Technical requirements
- Repository is in the zip file attached.
- The base project uses Lombok, so you must install it. You can use the following guide https://www.baeldung.com/lombok-ide
- The API must follow REST standard
- Use an in-memory database, such as H2 or similar.
- Write tests

## Recommended
- Improve the project (update the versions of the dependencies, Java JDK, gitignore, etc...)
- Add Docker Compose for local development
- Test coverage 80% or above
- Meaningful project description and instructions (README)
- API documentation (Swagger or similar)

## Considerations
The data model to be used is completely free, but as a minimum it must contain the following data:
- Basic Client info:
  o First and last name
  o Telephone number
- Basic Order info:
  o Order number (server side generated)
  o Delivery address
  o Number of pilotes
  o Order total (server side generated, consider 1.33 € as price for a single pilotes)

## Test evaluation

In this test, Quality is just as important as the correct implementation of specs. Take your time to produce a project that shows your best and respects the best practices. You could take inspiration from the most famous Open Source projects.

Compliance with specs and technical requirements are mandatory to pass the test.

The recommendations aren’t mandatory but concur to the final evaluation to bring you to the top of seniority.

## Test delivery

Use git and send us the repository using a bundle (as email attachment). You can use the following command to create the bundle:
```bash
git bundle create <yourname>.bundle --all –branches
```

Your reviewer will extract your git bundle with the command
```bash
git clone <yourname.bundle> projectDir
```

Please verify that the extraction works, before submitting it.


## NOTES

**_NOTE_**: Please, don’t share this exercise with anyone. 😉😉

**_NOTE2_**: The base project uses lombok, so you have to install it. You can use the following guide https://www.baeldung.com/lombok-ide

