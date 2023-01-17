# clj-error-log

```
-----> Building on the Heroku-22 stack
-----> Using buildpack: heroku/clojure
-----> Clojure app detected
-----> Installing OpenJDK 1.8... done
-----> Installing rlwrap... 
       Get:1 http://apt.postgresql.org/pub/repos/apt jammy-pgdg InRelease [91.6 kB]
       Get:2 http://archive.ubuntu.com/ubuntu jammy InRelease [270 kB]
       Get:3 http://apt.postgresql.org/pub/repos/apt jammy-pgdg/main amd64 Packages [418 kB]
       Get:4 http://archive.ubuntu.com/ubuntu jammy-security InRelease [110 kB]
       Get:5 http://archive.ubuntu.com/ubuntu jammy-updates InRelease [114 kB]
       Get:6 http://archive.ubuntu.com/ubuntu jammy/universe amd64 Packages [17.5 MB]
       Get:7 http://archive.ubuntu.com/ubuntu jammy/main amd64 Packages [1,792 kB]
       Get:8 http://archive.ubuntu.com/ubuntu jammy-security/main amd64 Packages [729 kB]
       Get:9 http://archive.ubuntu.com/ubuntu jammy-security/universe amd64 Packages [786 kB]
       Get:10 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 Packages [990 kB]
       Get:11 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 Packages [1,043 kB]
       Fetched 23.8 MB in 3s (9,272 kB/s)
       Reading package lists...
W: http://apt.postgresql.org/pub/repos/apt/dists/jammy-pgdg/InRelease: Key is stored in legacy trusted.gpg keyring (/etc/apt/trusted.gpg), see the DEPRECATION section in apt-key(8) for details.
       Reading package lists...
       Building dependency tree...
       The following NEW packages will be installed:
         rlwrap
       0 upgraded, 1 newly installed, 0 to remove and 4 not upgraded.
       Need to get 98.2 kB of archives.
       After this operation, 309 kB of additional disk space will be used.
       Get:1 http://archive.ubuntu.com/ubuntu jammy/universe amd64 rlwrap amd64 0.43-1build3 [98.2 kB]
       Fetched 98.2 kB in 0s (252 kB/s)
       Download complete and in download only mode
-----> Installing Clojure 1.10.0.411 CLI tools
       Downloading and expanding tar
       Installing libs into /tmp/build_93bbc361/.heroku/clj/lib/clojure
       Installing clojure and clj into /tmp/build_93bbc361/.heroku/clj/bin
       Installing man pages into /tmp/build_93bbc361/.heroku/clj/share/man/man1
       Removing download
       Use clj -h for help.
 !     WARNING: No :min-lein-version found in project.clj; using 1.7.1.
         You probably don't want this!
-----> Installing Leiningen
       Downloading: leiningen-1.7.1-standalone.jar
       To use Leiningen 2.x, add this to project.clj: :min-lein-version "2.0.0"
       Writing: lein script
-----> Building with Leiningen
       Running: lein deps
       Downloading: org/clojure/clojure/1.4.0/clojure-1.4.0.pom from repository central at http://repo1.maven.org/maven2
       Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/org/clojure/clojure/1.4.0/clojure-1.4.0.pom
       [WARNING] Unable to get resource 'org.clojure:clojure:pom:1.4.0' from repository central (http://repo1.maven.org/maven2): Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/org/clojure/clojure/1.4.0/clojure-1.4.0.pom
       Downloading: org/clojure/clojure/1.4.0/clojure-1.4.0.pom from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - RETRYING
       Downloading: org/clojure/clojure/1.4.0/clojure-1.4.0.pom from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - IGNORING
       [WARNING] POM for 'org.clojure:clojure:pom:1.4.0:compile' is invalid.
       
       Its dependencies (if any) will NOT be available to the current build.
       Downloading: compojure/compojure/1.1.1/compojure-1.1.1.pom from repository central at http://repo1.maven.org/maven2
       Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/compojure/compojure/1.1.1/compojure-1.1.1.pom
       [WARNING] Unable to get resource 'compojure:compojure:pom:1.1.1' from repository central (http://repo1.maven.org/maven2): Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/compojure/compojure/1.1.1/compojure-1.1.1.pom
       Downloading: compojure/compojure/1.1.1/compojure-1.1.1.pom from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - RETRYING
       Downloading: compojure/compojure/1.1.1/compojure-1.1.1.pom from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - IGNORING
       [WARNING] POM for 'compojure:compojure:pom:1.1.1:compile' is invalid.
       
       Its dependencies (if any) will NOT be available to the current build.
       Downloading: ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.pom from repository central at http://repo1.maven.org/maven2
       Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.pom
       [WARNING] Unable to get resource 'ring:ring-jetty-adapter:pom:1.1.2' from repository central (http://repo1.maven.org/maven2): Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.pom
       Downloading: ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.pom from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - RETRYING
       Downloading: ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.pom from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - IGNORING
       [WARNING] POM for 'ring:ring-jetty-adapter:pom:1.1.2:compile' is invalid.
       
       Its dependencies (if any) will NOT be available to the current build.
       Downloading: compojure/compojure/1.1.1/compojure-1.1.1.jar from repository central at http://repo1.maven.org/maven2
       Downloading: ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.jar from repository central at http://repo1.maven.org/maven2
       Downloading: org/clojure/clojure/1.4.0/clojure-1.4.0.jar from repository central at http://repo1.maven.org/maven2
       Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/compojure/compojure/1.1.1/compojure-1.1.1.jar
       [WARNING] Unable to get resource 'compojure:compojure:jar:1.1.1' from repository central (http://repo1.maven.org/maven2): Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/compojure/compojure/1.1.1/compojure-1.1.1.jar
       Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.jar
       [WARNING] Unable to get resource 'ring:ring-jetty-adapter:jar:1.1.2' from repository central (http://repo1.maven.org/maven2): Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.jar
       Downloading: compojure/compojure/1.1.1/compojure-1.1.1.jar from repository clojars at http://clojars.org/repo/
       Downloading: ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.jar from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/org/clojure/clojure/1.4.0/clojure-1.4.0.jar
       [WARNING] Unable to get resource 'org.clojure:clojure:jar:1.4.0' from repository central (http://repo1.maven.org/maven2): Error transferring file: Server returned HTTP response code: 501 for URL: http://repo1.maven.org/maven2/org/clojure/clojure/1.4.0/clojure-1.4.0.jar
       Downloading: org/clojure/clojure/1.4.0/clojure-1.4.0.jar from repository clojars at http://clojars.org/repo/
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - RETRYING
       Downloading: compojure/compojure/1.1.1/compojure-1.1.1.jar from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - RETRYING
       Downloading: ring/ring-jetty-adapter/1.1.2/ring-jetty-adapter-1.1.2.jar from repository clojars at http://clojars.org/repo/
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - IGNORING
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - RETRYING
       Downloading: org/clojure/clojure/1.4.0/clojure-1.4.0.jar from repository clojars at http://clojars.org/repo/
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - IGNORING
       Transferring 0K from clojars
       [WARNING] *** CHECKSUM FAILED - Checksum failed on download: local = '1965c4952cc8c082a6307ed67061a57aab6632fa'; remote = '<html>
       <head><title>301' - IGNORING
       Copying 3 files to /tmp/build_93bbc361/lib
       Exception in thread "main" java.lang.RuntimeException: java.util.zip.ZipException: error in opening zip file (NO_SOURCE_FILE:0)
       	at clojure.lang.Compiler.eval(Compiler.java:5440)
       	at clojure.lang.Compiler.eval(Compiler.java:5391)
       	at clojure.core$eval.invoke(core.clj:2382)
       	at clojure.main$eval_opt.invoke(main.clj:235)
       	at clojure.main$initialize.invoke(main.clj:254)
       	at clojure.main$script_opt.invoke(main.clj:270)
       	at clojure.main$main.doInvoke(main.clj:354)
       	at clojure.lang.RestFn.invoke(RestFn.java:457)
       	at clojure.lang.Var.invoke(Var.java:377)
       	at clojure.lang.AFn.applyToHelper(AFn.java:172)
       	at clojure.lang.Var.applyTo(Var.java:482)
       	at clojure.main.main(main.java:37)
       Caused by: java.lang.RuntimeException: java.util.zip.ZipException: error in opening zip file
       	at clojure.lang.LazySeq.sval(LazySeq.java:47)
       	at clojure.lang.LazySeq.seq(LazySeq.java:56)
       	at clojure.lang.RT.seq(RT.java:450)
       	at clojure.core$seq.invoke(core.clj:122)
       	at leiningen.deps$extract_native_deps.invoke(deps.clj:174)
       	at leiningen.deps$deps.doInvoke(deps.clj:200)
       	at clojure.lang.RestFn.invoke(RestFn.java:410)
       	at clojure.lang.Var.invoke(Var.java:365)
       	at clojure.lang.AFn.applyToHelper(AFn.java:161)
       	at clojure.lang.Var.applyTo(Var.java:482)
       	at clojure.core$apply.invoke(core.clj:542)
       	at leiningen.core$apply_task.invoke(core.clj:262)
       	at leiningen.core$_main.doInvoke(core.clj:329)
       	at clojure.lang.RestFn.invoke(RestFn.java:410)
       	at clojure.lang.AFn.applyToHelper(AFn.java:161)
       	at clojure.lang.RestFn.applyTo(RestFn.java:132)
       	at clojure.core$apply.invoke(core.clj:542)
       	at leiningen.core$_main.invoke(core.clj:332)
       	at user$eval42.invoke(NO_SOURCE_FILE:1)
       	at clojure.lang.Compiler.eval(Compiler.java:5424)
       	... 11 more
       Caused by: java.util.zip.ZipException: error in opening zip file
       	at java.util.zip.ZipFile.open(Native Method)
       	at java.util.zip.ZipFile.<init>(ZipFile.java:233)
       	at java.util.zip.ZipFile.<init>(ZipFile.java:162)
       	at java.util.jar.JarFile.<init>(JarFile.java:173)
       	at java.util.jar.JarFile.<init>(JarFile.java:137)
       	at sun.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method)
       	at sun.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:62)
       	at sun.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45)
       	at java.lang.reflect.Constructor.newInstance(Constructor.java:423)
       	at clojure.lang.Reflector.invokeConstructor(Reflector.java:160)
       	at leiningen.deps$extract_native_deps$fn__2418.invoke(deps.clj:174)
       	at clojure.core$map$fn__3699.invoke(core.clj:2096)
       	at clojure.lang.LazySeq.sval(LazySeq.java:42)
       	... 30 more
```
