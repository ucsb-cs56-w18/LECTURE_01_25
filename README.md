# LECTURE_01_25
Thursday

# What happens when you do `git clone`

When you type this command:

```
git clone git@github.com:UCSB-CS56-pconrad/cs56-rational-ex04.git
```

It is the same as:
* `mkdir cs56-rational-ex04`
* `cd cs56-rational-ex04`
* `git init`
   * turns a regular Unix directory (or Mac or Windows folder) into a git repo
* `git remote add origin git@github.com:UCSB-CS56-pconrad/cs56-rational-ex04.git`
   * adds a remote called `origin` that points back to that particular url
  
The point is: these are equivalent processes.  

# Where to get the JUnit jar from

One place is: https://www.cs.ucsb.edu/~pconrad/cs56/lib/

Or on CSIL, the directory

```
/cs/faculty/pconrad/public_html/cs56/lib/
```


# Maven

* <https://maven.apache.org/guides/getting-started/>

When you see:

```
mvn -B archetype:generate \
  -DarchetypeGroupId=org.apache.maven.archetypes \
  -DgroupId=com.mycompany.app \
  -DartifactId=my-app
```

It should be:

```
mvn -B archetype:generate \
  -DarchetypeGroupId=org.apache.maven.archetypes \
  -DgroupId=edu.ucsb.cs56.w18.yourgithubid.myapp \
  -DartifactId=my-app
```

And really, it should be as follows (the `\` are just there to show that the command line is too long to fit on a single line.

```
mvn -B archetype:generate -DarchetypeGroupId=org.apache.maven.archetypes -DgroupId=edu.ucsb.cs56.w18.yourgithubid.myapp -DartifactId=my-app
```

# Making the jar executable

* <https://maven.apache.org/shared/maven-archiver/examples/classpath.html>

