#Problem

We want to take a list of MP3s, determine the ideal transitions between each corresponding MP3, and generate a single MP3 file which is a mashup of all of the MP3s.  Between each transition, the tempo of the song is slowly altered to match the tempo of the song it transitions to.

#Questions

How do you determine the ideal transitions?

What happens if a taken transition is further in the song transitioned to than the ideal transition to the next song?

How do you take all these MP3 files and convert them into one MP3 file?

How can these problems be solved as quickly as possible?

#Resources

1: [twosongshift.py]
2: [The Infinite Jukebox]
3: [mp3combine.py]

###Mini-abstract and relevance of [twosongshift.py]

A python script I previously wrote already solves the problem of determining the ideal transition between 2 songs.  Using an algorithm similar to [The Infinite Jukebox], [twsongshift.py] determines a transition based on the weighted euclidean distances of 2 segments between their timbre, pitch, and volume.

###Mini-abstract and relevance of [The Inifinite Jukebox]

The Infinite Jukebox has been the basis of this research problem for the past few months.  It is a piece of software that plays a song continuously, taking transitions between segments that are similar in their pitch, timbre, duration, and loudness.  This comparison is done with a weighted euclidean distance.  This technique can be extended to our problem to fix the issue where a song begins playing at a point past the best transition to the next song.

###Mini-abstract and relevance of [mp3combine.py]

mp3combine.py was a simple script I wrote to take a list of MP3 files and combine them into one file.  Although this was a very simple task, I realized that this can be done in a much more efficient way than it had been before.  Due to the large amounts of data that will be handled by these questions, this increase in speed is a necessity for solving these problems.

[twosongshift.py]: https://github.com/mulfordjc/TwoBeatShift/blob/master/twosongshift.py
[The Infinite Jukebox]: infinitejuke.com
[mp3combine.py]: https://github.com/mulfordjc/MP3Repository/blob/master/mp3combine.py
