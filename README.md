# DSC Tournament
Web-based interface for the results of the DARPA Spectrum Challenge

## Auto-commiting changes

On a linux server, use the following line for triggering a git commit 
automatically, whenever the file(s) have changed

    inotifywait -q -m -e CLOSE_WRITE --format="git commit -m 'autocommit on change' %w" results.yaml | sh

You might need to install `inotify-tools` before:

    sudo apt-get install inotify-tools