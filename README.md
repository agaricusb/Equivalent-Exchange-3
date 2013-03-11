## Welcome to Equivalent Exchange 3!
**LATEST OFFICIAL VERSION**:  [EE3 pre1f for Minecraft 1.4.6/1.4.7] (http://adf.ly/GjT3c)

[Minecraft Forums page] (http://www.minecraftforum.net/topic/1540010-equivalent-exchange-3)

[Compiling EE3] (https://github.com/pahimar/Equivalent-Exchange-3#compiling-equivalent-exchange-3) - For those that want the latest unreleased features.

[Contributing] (https://github.com/pahimar/Equivalent-Exchange-3#contributing) - For those that want to help out.

### Compiling Equivalent Exchange 3
IMPORTANT: This is not guaranteed to work as it has not been tested extensively (Linux and Windows tested).
***
#### Prerequisites  (Tested for Windows ONLY!)
1. **WARNING:  Make sure you know EXACTLY what you're doing!  It's not any of our faults if your OS crashes, becomes corrupted, etc.**
2. Download and install the Java JRE [here] (http://www.java.com/inc/BrowserRedirect1.jsp?locale=en) (necessary for Maven).
3. Download and install the Java JDK [here] (http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html).  Scroll down, accept the `Oracle Binary Code License Agreement for Java SE`, and download the one pertaining to your OS (necessary for MCP).
	* Go to `Control Panel\System and Security\System`, and click on `Advanced System Settings` on the left-hand side.
	* Click on `Environment Variables`.
  * Under `System Variables`, click `New`.
  * For `Variable Name`, input `JAVA_HOME`.
  * For `Variable Value`, input something similar to `;C:\Program Files (x86)\Java\jdk1.7.0_11` exactly as shown to the end (or wherever your Java JDK installation is), and click `Ok`.
  * Scroll down to a variable named `Path`, and double-click on it.
  * Append `;C:\Program Files (x86)\Java\jdk1.7.0_11\bin` (or wherever your Java JDK installation is \bin), and click `Ok`.
4. Download Apache Maven [here] (http://maven.apache.org).
	* Unzip the files anywhere you want, eg `C:\Program Files (x86)\Maven`.
  * Again, go to `Environment Variables` just like you did for the Java JDK.
  * Under `System Variables`, click `New`.
  * TODO
5. Download and install Github [here] (http://windows.github.com/) (Windows) or [here] (http://mac.github.com/) (Mac OS X 10.7+).  For Linux, I *guess* you could download it as a .zip/tarball and unzip it?
	* Create an account.
  * Scroll to the top of this page, login at the top-right, and then click `Clone to Windows/Mac` near the top-left of the page.
  * You should see Github flash and `pahimar/Equivalent-Exchange-3` appear.  (The local repository on Windows defaults to `C:\Users\(username)\Documents\GitHub\Equivalent-Exchange-3`, you can change it if you want but then you have to find it again on Github).


#### Setup EE3 (Some tested for Linux, tested fully for Windows)
1. Right now, you should have a directory that looks something like:

***
		\-Equivalent-Exchange-3
			\-EE3's files (should have pom.xml).
***

2. [FOR WINDOWS] Open up `cmd` by typing `cmd` in Run.
3. [FOR WINDOWS] Navigate to `Equivalent-Exchange-3` by executing `cd Equivalent-Exchange-3`.
4. Execute `mvn initialize -P -built`. This will generally take around 15-30 seconds, depending on your computer.  If you've done everything right, `BUILD SUCCESSFUL` is displayed after it finishes
5. Execute `mvn package`. This will generally take around 3-5 seconds, depending on your computer.  If you've done everything right, `BUILD SUCCESSFUL` is displayed after it finishes.
	* If you see `BUILD FAILED`, check the error output (it should be right around `BUILD FAILED`), fix everything, and try again.
6. Go to `Equivalent-Exchange-3\target`
	*  You should see a .jar named `ee3-pre2.jar`.
7. Copy the jar into your Minecraft mods folder, and play Minecraft!

#### Updating Your Repo (For Windows/Mac)
1. Check to see if pahimar updated EE3 since you last compiled.  If he did, follow these instructions.
2. Open Github.
3. Double-click on pahimar/Equivalent-Exchange-3.
4. At the top, there is a button named `Sync`/`Sync Branch` (Mac) (or `Refreshing...` if it's still checking).
5. Click `Sync`, and wait for it to finish.
6. Re-compile

###Contributing
***
#### Submitting a PR
So you found a bug in pahimar's code?  Think you can make it more efficient?  Want to help in general?  Great!

1. **IMPORTANT:  PAHIMAR DOES *NOT* WANT ANY** `pom.xml` **CHANGES, UNLESS it fixes up something broken** (See [Pull Request #90] (https://github.com/pahimar/Equivalent-Exchange-3/pull/90)).
2. If you haven't already, create a Github account.
3. Click the little branch/plus icon at the top-right of this page (below your username).
4. Make the changes that you want to.
5. Click `Pull Request` at the top-middle of the page (left of your fork's name, to the right of `Watch` and `Fork`).
6. Enter your PR's title, and create a detailed description telling pahimar what you changed.
7. Click `Send pull request`, and you're done!

#### Creating an Issue
EE3 crashes every time?  Have a suggestion?  Found a bug?  Create an issue now!

1. Go to [the issues page] (http://github.com/pahimar/Equivalent-Exchange-3/issues).
2. Click `New Issue` right below `Graphs`.
3. Enter your Issue's title (something that summarizes your issue), and then create a detailed description ("Hey pahimar, could you add/change xxx?" or "Hey, found an exploit:  stuff").
4. Click `Submit new issue`, and you're done!
