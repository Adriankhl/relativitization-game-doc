# Frequently asked questions

### Will this be on Steam?

Yes, after it is more polished. At least I am planning to add Chinese translation for the game before Steam release.

### Why the android apk is experimental?

In principle, this game should work on android phones. However, due to the heavy computation, it might not be a pleasant
experience to player this game on android. Optimization might be possible int the future to provide a smooth experience
on android.

### Game crashes to desktop?

Possible reasons:

* The memory allocated to the game is not sufficient, e.g., you are playing with a huge map
    * Start your game with a smaller universe
    * (Windows only): open `app/relativitization-win.cfg` and modify `java-options=-XX:MaxRAMPercentage=50` from 50 to a
      larger number
* Your game uses too much memory, your OS kills the process automatically
    * Close some of your other memory-intensive applications while playing
    * (Windows only): open `app/relativitization-win.cfg` and modify `java-options=-XX:MaxRAMPercentage=50` from 50 to a
      smaller number