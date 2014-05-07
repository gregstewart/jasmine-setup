Jasmine setup with Istanbul code coverage
=============

Since I run through these steps on nearly every project here's a base line setup to build on. It uses Grunt, Karma, Jasmine,
JSHint and the global name space checker spec

To get started simply cd into the project root and type:

    npm install

Then you can simply type:

    grunt
    
And then you should see something like this:

    Running "jshint:all" (jshint) task
    >> 3 files lint free.

    Running "karma:unit" (karma) task
    INFO [karma]: Karma v0.10.10 server started at http://localhost:9876/
    INFO [launcher]: Starting browser PhantomJS
    INFO [PhantomJS 1.9.7 (Windows 8)]: Connected on socket fkoSEVT4nQMxYwPokTjT
    PhantomJS 1.9.7 (Windows 8): Executed 6 of 6 SUCCESS (0.172 secs / 0.024 secs)

    =============================== Coverage summary ===============================
    Statements   : 93.33% ( 14/15 )
    Branches     : 100% ( 2/2 )
    Functions    : 85.71% ( 6/7 )
    Lines        : 93.33% ( 14/15 )
    ================================================================================

If you want to plug this into your WebStorm IDE:

 1. Go to "Edit configurations"
 2. Add a new configuration for Node.js
 3. Give it name e.g.: "Karma"
 4. Specify the fully qualified path to your Node executable: "C:\Program Files\nodejs\node.exe"
 5. Path to your Karma installation, e.g.: C:\projects\Github\jasmine-setup\node_modules\karma
 6. Application start parameters: C:\projects\Github\jasmine-setup\karma.conf.js


