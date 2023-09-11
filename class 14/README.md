## Intro to password hashing

### Define the term “hashing”.?

chopping something into small pieces 

### Explain to a non-technical friend what a hash function does to a password.
it switches the password of any length into a certain constant length of a string to protect the data with any small change in the input value resulting in huge changes to the result 

## bcrypt overview

### What does it mean to ‘salt’ a password?
a ‘salt’ adds a very long string of bytes to the password

### What piece of information would a hacker need to access in order to find the ‘salt’ string for your passwords?
 
your source code 

## jBCrypt (the paragraphs and code example at the top of the page)

### How does the Blowfish block cipher handle the increased computation speed of new computers?

This system hashes passwords using a version of Bruce Schneier's Blowfish block cipher with modifications designed to raise the cost of off-line password cracking and frustrate fast hardware implementation

### What are the issue with the two most commong password hashes for Java (“Java password hash” and “Java password encryption”)?

 "Java password hash" and "Java password encryption" both offer terrible advice: one uses an unsalted hash which allows reverse dictionary lookup of passwords and the other recommends reversible encryption, which is rarely needed and should only be used as a last resort.
