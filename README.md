Maven repository for all my projects


======================================
To deploy jar manually to this repository
======================================
1. run the command

<pre><code>
 mvn deploy:deploy-file 
 -DgroupId=your-group-id
 -DartifactId=your-artifact-id 
 -Dversion=1.0 
 -Dpackaging=jar 
 -Dfile=path/to/file/jar_name.jar 
 -Durl=file:///path/to/local/maven-repo/releases/
</code></pre>

* jar example
<pre><code>
  mvn deploy:deploy-file 
  -DgroupId=in.github.vteial
  -DartifactId=myutils 
  -Dversion=1.0 
  -Dpackaging=jar 
  -Dfile=myutils.jar
  -Durl=file:///users/vteial/git/maven-repo/releases/
</code></pre>

* pom example 
<pre><code>
 mvn deploy:deploy-file 
 -DgroupId=io.github.vteial
 -DartifactId=reporting
 -Dversion=1.0 
 -Dpackaging=pom 
 -Dfile=reporting/pom.xml 
 -Durl=file:///users/vteial/git/maven-repo/releases/
</code></pre>

2. push the changes
