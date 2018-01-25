# LECTURE_01_25
Thursday

# What happens when you do `git clone`

When you type this command:

```
git clone git@github.com:UCSB-CS56-pconrad/cs56-rational-ex04.git
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
