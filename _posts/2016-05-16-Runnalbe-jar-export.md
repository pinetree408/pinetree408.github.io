---
layout: post
maintitle: Runnable jar export
subtitle: Runnable jar export with text file in source tree
---

## What issuse

When i exported runnable jar, jar has error with read text file in source directory

## How to study

Change File Reader to InputStreamReader for read texf file.
In case, those text file is in src.

```
file  = "/example.txt";

InputStream input = [ClassName].class.getResourceAsStream(file);

BufferedReader in = new BufferedReader(new InputStreamReader(input));

while ((s = in.readLine()) != null) {
	...
}
```
