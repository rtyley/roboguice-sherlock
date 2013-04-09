# roboguice-sherlock [![Build Status](https://travis-ci.org/rtyley/roboguice-sherlock.png)](https://travis-ci.org/rtyley/roboguice-sherlock)

**RoboGuice classes for use with ActionBarSherlock**

Both RoboGuice and ActionBarSherlock require custom base classes for Activities
and Fragments, and as Java doesn't permit diamond-inheritance, or the [traits](http://www.scala-lang.org/node/126)
of Scala, this project provides custom RoboGuice classes that extend the corresponding
ones from ActionBarSherlock.

[JakeWharton](https://github.com/JakeWharton) provided the first example of how
to do this with a [RoboSherlockActivity](https://github.com/JakeWharton/ActionBarSherlock/blob/4.0.0/samples/roboguice/src/com/actionbarsherlock/sample/roboguice/RoboSherlockActivity.java):
it's a simple drudge process of taking the source for the RoboGuice class and
changing the activity/fragment named in the `extends` declaration to the
corresponding ActionBarSherlock class - there are no further complications
I've encountered so far.

All classes in this project have the same name as the RoboGuice ones, with 'Sherlock'
inserted after the 'Robo', ie `Robo**Sherlock**ListFragment`. The package is also changed
to `com.github.rtyley.android.sherlock.roboguice.**`.

Download releases from Maven:

http://search.maven.org/#search%7Cgav%7C1%7Cg%3A%22com.github.rtyley%22%20AND%20a%3A%22roboguice-sherlock%22

## Used in...

The open-source [Gaug.es](https://play.google.com/store/apps/details?id=com.github.mobile.gauges)
web analytics app by GitHub.

