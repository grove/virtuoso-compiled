
Start up a CoreOS instance using vagrant.
<pre>
vagrant up
</pre>

Then log in to the VM using ssh:
<pre>
vagrant ssh
</pre>

Now you can spin up a Docker container containing Virtuoso 7 Open Source edition.

<pre>
$ docker run -i -t -p 8890:8890 grove/virtuoso-compiled /usr/local/virtuoso-opensource/bin/virtuoso-t -df +configfile /usr/local/virtuoso-opensource/var/lib/virtuoso/db/virtuoso.ini
</pre>

Open the Sparql endpoint in your browser. Enjoy!

<pre>
http://localhost:8890/sparql
</pre>

