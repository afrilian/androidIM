AndroidIM

###How to make it run:

    WebAPI:
        There is a folder whose name is "android-im_WEBAPI", copy all files under "android-im" folder to a folder in            
        your web server directory, 
        for instance android-im that can be accessed by http://192.168.7.5/android-im/ (192.168.7.5 is the IP address of 
        computer which runs apache and mysql, 
        use local network IP address instead of using localhost or 127.0.0.1).
        Open the index.php and enter database connectivity parameters such as host, username, password etc. write 
        error_reporting(0) in top of index.php
        Create the tables in mysql database with the included android_im.sql
        
    Android APP:
        set AUTHENTICATION_SERVER_ADDRESS in socketOperator, it must be the address where server folder are located,
        for our example it is http://192.168.7.5/android-im/ (don't use localhost)
        
    Then run your application in Eclipse with ADT plugin.
    it can be learned how to install Android SDK and ADT plugin.
