Creating a New App with Yeoman
=======================

Yeoman is a scaffolding tool that provides generators for apps with BackboneJS, AngularJS, EmberJS, Wordpress themes and more.

Yeoman scaffolds out a new application, writing your Grunt configuration and pulling in relevant Grunt tasks and Bower dependencies that you might need for your build.

Grunt is used to build, preview and test your project, thanks to help from tasks curated by the Yeoman team and grunt-contrib. GulpJS is an alternative to Grunt, but has little support at the moment: http://gulpjs.com/

Bower is used for dependency management, so that you no longer have to manually download and manage your scripts.

Getting Started
---

1. Install node.js: http://nodejs.org

    To avoid using ```sudo``` when installing packages, run the following:

    ```
        sudo chown -R `whoami` ~/.npm
        sudo chown -R `whoami` /usr/local/lib/node_modules
    ```

2. Install Yeoman, grunt-cli and Bower

    ```
        npm install -g yo
        npm install -g grunt-cli
        npm install -g bower
    ```

3. Install the needed generators, generator-webapp is used by default
    
    ```
        npm install -g generator-webapp
    ```

4. Create a project folder, enter it and run:

    ```    
        yo webapp <<app-name>>
    ```

5. Run the grunt server task:

    ```
        grunt serve
    ```

6. And for the build task:

    ```
        grunt build
    ```
    
7. To install packages add them to the bower.json file and run:

    ```
        bower install
    ```
    
    Alternatively, run:
    
    ```
        bower install --save <<package-name>>
    ```
    
    Visit http://bower.io/search/ for a list of available packages

References
---
* http://nodejs.org/
* http://yeoman.io/
* http://bower.io/
* http://gruntjs.com/getting-started