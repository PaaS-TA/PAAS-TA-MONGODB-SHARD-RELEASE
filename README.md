## PAAS-TA-MONGODB-SHARD-RELEASE  

### PaaS-TA MongoDB Shard Release Configuration   
  - mongodb_broker : 1 machine  
  - mongodb_shard : 1 machine  
  - mongodb_config : N machine(s)  
  - mongodb_master : N machine(s)  
  - mongodb_slave : N machine(s)  

### Create PaaS-TA MongoDB Shard Release  
  - Download the latest PaaS-TA MongoDB Shard Release  
    ```  
    $ git clone https://github.com/PaaS-TA/PAAS-TA-MONGODB-SHARD-RELEASE.git  
    $ cd PAAS-TA-MONGODB-SHARD-RELEASE  
    ```  
  - Create PaaS-TA MongoDB Shard Release  
    ```  
    ## <VERSION> :: release version (e.g. 2.0.1)
    ## <RELEASE_TARBALL_PATH> :: release file path (e.g. /home/ubuntu/workspace/paasta-mongodb-shard-<VERSION>.tgz)
    $ bosh -e <bosh_name> create-release --name=paasta-mongodb-shard --version=<VERSION> --tarball=<RELEASE_TARBALL_PATH> --force

    ```   
