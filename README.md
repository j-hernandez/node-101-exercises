## Training Exercises

### Small

#### Launch Node

Run `node` in the terminal and `console.log()` the string "Hello World."


#### Hello Node

* Create an `index.js` file, and have it `console.log()` the string "Hello World, I am in Node."
* Run `node` and execute the file.


#### Hello World Server

Create a "hello world" server using the `http` module that starts a server and returns plain text.


#### Using `npm`

Print out the version of `npm` that you have installed


#### Initialize a new package

Create a new folder called `cowsay-practice` and initialize `npm`


#### Cowsay

Install the [cowsay package](https://www.npmjs.com/package/cowsay) and call `cowsay.say()`.


### Medium

#### DNS Lookup

Write a program that prompts the user for a domain name, looks up the IP address for the domain, and prints it out.

Example Output:

```sh
$ node dns_lookup.js
Domain Name: google.com
IP Address:  172.217.2.46
```

Trigger an error condition by providing an invalid domain. See that the error gets displayed.

HINT
Node has a built in module called `dns`.  It has quite a few helpful methods, such as `lookup()`.


#### Read a File

Write a program that prompts the user to enter a file name, and reads in the contents of the file, convert the text to all caps, and prints it out.

Assuming the file `file1.txt` contains the text: "Hello, I am file 1."

Example output:

```sh
$ node read_file.js
filename: file1.txt
HELLO, I AM FILE 1.
```

Trigger an error condition by running the program on a non-existent file. Your program should display the error message, and it should display something like:

```sh
$ node read_file.js
filename: blah.txt
ENOENT: no such file or directory, open 'blah.txt'
```

HINT
There are two Node modules that are part of Node code that will help with this exercise, `readline` and `fs`.

- The `fs` module is provides a lot of helpful functionality when working with the file system. There are a variety of file related methods, such as `readFile()` and `writeFile()` that you will helpful.
- The `readline` module has quite a few helpful methods for reading input.  In particular, there is the `question()` method that waits for user input.




#### Read AND Write to a File

Write a program to prompt the user for two file names, the first file will be the input and the second file will be the output. The program will read in the contents of the input file, convert its text to all caps, and then write the resulting contents to the output file.

Example Output:

```sh
$ node read_and_write_file.js
Input file: file1.txt
Output file: output.txt
Wrote to file output.txt
As a result, output.txt should now contain the text HELLO, I AM FILE 1
```

Trigger an error by running the program with an non-existing input file, ensure that the error is properly displayed. Trigger an error by running the program with an output file in a non-existant directory, such as thisdirdoesntexist/output.txt, ensure that the error is properly displayed.

