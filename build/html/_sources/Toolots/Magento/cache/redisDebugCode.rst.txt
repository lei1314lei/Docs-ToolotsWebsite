Debug Code For redis type cache backed
======================================

.. code-block:: php

       $backendOptions = array(
            'server' => '192.168.10.254',
            'port' => 6379,
            'persistent' => null,
            'database' => 0,
            'password' =>null ,
            'force_standalone' => 0,
            'connect_retries' => 5,
            'read_timeout' => 10,
            'automatic_cleaning_factor' => 0,
            'compress_data' => 1,
            'compress_tags' => 1,
            'compress_threshold' => 20480,
            'compression_lib' =>'gzip',
            'use_lua' => 0
        );
       $backend = new Cm_Cache_Backend_Redis($backendOptions);
       $id ='7c9_BLOCK_TOOLOTS_CATALOG_BLOCK_DEALOFMONTHPRODUCTS_1_1';
       $data = $backend->load($id);
       echo $data;



