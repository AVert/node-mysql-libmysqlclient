NodeJS mysql-sync bindings API
==============================

Introduction
------------

This file contains overview of node-mysql-sync API.


MysqlSyncConn class
-------------------

    class MysqlSyncConn {
        /* Constructor */
        require('mysql-sync').createConnection(servername, user, password, dbname, port, socket);
        
        /* Methods */
        Integer affectedRows();
        Boolean changeUser(user, password, dbname);
        Boolean connect(hostname, user, password, dbname, port, socket);
        Integer connectErrno();
        String connectError();
        Boolean close();
        Integer errno();
        String error();
        String escape();
        Object getInfo();
        Integer lastInsertId();
        Boolean ping();
        MysqlSyncRes query();
        Integer warningCount();
    }


Connection, options, errors and information
-------------------------------------------

### Connection ###

    require('mysql-sync').createConnection(servername, user, password, dbname, port, socket);
    
    Boolean changeUser(user, password, dbname);
    Boolean connect(hostname, user, password, dbname, port, socket);
    Integer connectErrno();
    String connectError();
    Boolean close();
    Object getCharset();
    String getCharsetName();
    Boolean ping();
    Boolean selectDb (dbname);
    Boolean setCharset (charset);
    Undefined setSsl(key, cert, ca, capath, cipher);
    

### Options ###

Nothing yet.


### Errors ###

    Integer errno();
    String error();


### Information ###

    Object getInfo();
    Integer warningCount();


Query
-----

    Integer affectedRows();
    String escape(escapestr);
    Integer lastInsertId();
    MysqlSyncRes query(query);


Transactions
------------

Nothing yet.


Other
-----

Nothing yet.
