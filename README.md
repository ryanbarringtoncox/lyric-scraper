## Intro

I love the command line.  I love listening to music while I hack.  I love getting the lyrics to songs quickly.  It's a pain to fire up a browser, type a lyrics search into google, wade through the results, copy and paste.  You get the idea.

I spent a few hours trying out a few supposed lyric apis and had no luck.  I want lyrics quick and easy from the command line in one command.  Why not script what I've been doing?

## Install

You are encouraged to use virtualenv

    sudo pip install virtualenv
    git clone https://github.com/ryanbarringtoncox/command_line_lyrics
    cd command_line_lyrics/
    virtualenv env
    source env/bin/activate
    pip install lxml requests 

You'll also need Ruby and ruby-web search.

    gem install ruby-web-search

## Grab lyrics from the web! 

Run the script and pass in the words that you'd use to find lyrics online.  **No punctuation please!** Some examples -

    ./command_line_lyrics.py the beatles in my life 
    ./command_line_lyrics.py blur tender
    ./command_line_lyrics.py buddy holly peggy sue 

And they'll stream by on the console for your reading pleasure.  You can also redirect them to a text file like this -

    ./command_line_lyrics.py rolling stones shine a light > shine-a-light.txt

