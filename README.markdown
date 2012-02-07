# Ruby Web Apps Tutorial - Jekyll

This source code is a [Jekyll](http://jekyllrb.com/) based website, and is also the notes + slides I wrote down to run my recent Intro to Rails workshop.

## Running locally

To view the notes, or to simply see how this Jekyll website works, you will need to download this code.

Open up your terminal and navigate to your projects directory or something similar, and `git pull` the source code:
    
    cd ~/projects
    git pull git://github.com/matholroyd/rwat-jekyll.git
    
Now change into the rwat-jekyll directory and make sure you have the necessary gems:

    cd rwat-jekyll
    bundle
    
Once the gems are installed, you can run this Jekyll app in development mode, meaning you make changes to the source code and see the changes when you refresh a page. To run Jekyll in development mode, run:

    jekyll --server
    
By default, the server will be accessible via `localhost:4000`


  
