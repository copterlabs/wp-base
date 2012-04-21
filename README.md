WordPress Base Install for Copter Labs Projects
===============================================

All the themes and plugins used by default in a 
[Copter Labs](http://www.copterlabs.com/) WordPress project.

Usage
-----

You may have noticed that this doesn't actually include the WordPress core.
We did that on purpose. [WordPress is already on GitHub](https://github.com/wordpress/wordpress), so you should be getting it from there.

### Installation

First, get into your web root. If you're using Media Temple as we so ofter do,
you might want to empty the folder to start.

#### Step 1. Clone the Latest Version of WordPress

    git clone git://github.com/WordPress/WordPress.git

#### Step 2. Move WordPress Into the Web Root Folder

    mv WordPress/* .
    rm -rf WordPress/

#### Step 3. Initialize Git and Load the WP Base

    git init
    git remote add origin git@github.com:copterlabs/wp-base.git
    git pull origin master

#### Step 4. Initialize Submodules and Update Them

    git submodule init
    git submodule update

#### Step 5. Create Your Child Theme and Create Your Stylesheet

    mkdir wp-content/themes/childtheme
    touch wp-content/themes/childtheme/style.css

_**NOTE:** You need to add the comment block to set this as a child theme. You can grab it from [our Gist here](https://gist.github.com/2439691) or from [the WordPress Codex](http://codex.wordpress.org/Child_Themes#The_required_style.css_file)._

#### Step 6. Dance.

Like this:

![Dancing kid](http://cptr.us/images/dance.gif)

Or this:

![Dancing Takei](http://cptr.us/images/takei.gif)

