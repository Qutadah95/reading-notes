## Packages and Import

Package = directory. Java classes can be grouped together in packages. A package name is the same as the directory (folder) name which contains the .java files


## Package declaration syntax

// This source file must be Drawing.java in the illustration directory.

package illustration;

import java.awt.*;

public class Drawing {
    . . .
}


## Java Loops


### For Loop

Syntax

for (statement 1; statement 2; statement 3) {
  // code block to be executed
}

Example:
for (int i = 0; i < 5; i++) {
  System.out.println(i);
}

### For-Each Loop

Syntax

for (type variableName : arrayName) {
  // code block to be executed
}

Example:

String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
for (String i : cars) {
  System.out.println(i);
}

### While Loop

Syntax

while (condition) {
  // code block to be executed
}

Example:

int i = 0;
while (i < 5) {
  System.out.println(i);
  i++;
}


### Do/While Loop 

Syntax:

do {
  // code block to be executed
}
while (condition);


Example:

int i = 0;
do {
  System.out.println(i);
  i++;
}
while (i < 5);