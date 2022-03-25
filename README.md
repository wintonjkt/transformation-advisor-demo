# Transformation Advisor Demo Setup
  
  
  
## Install and run WebSphere Application Server

  1. Download IBM Installation Manager for your OS from https://www.ibm.com/support/pages/installation-manager-19
  2. Install IBM Installation Manager, extract the downloaded zip file, and run install
  3. Add WebSphere 9.0 repository to IBM Installation Manager, we use WAS Base http://www.ibm.com/software/repositorymanager/com.ibm.websphere.BASE.v90
     Full reference: https://www.ibm.com/docs/en/was/9.0.5?topic=installation-online-product-repositories-websphere-application-server-offerings
  4. Open Profile Management Tool and create an Application Server Profile
  5. Default root of AppServer is /opt/IBM/WebSphere/AppServer/bin
  6. Start / Stop WAS
     View the status of WebSphere Application Server, go to the [appserver root]/bin directory and run ./serverStatus.sh server_name
     Start WebSphere Application Server, go to the [appserver root]/bin directory and run ./startServer.sh server_name
     Stop WebSphere Application Server, go to the [appserver root]/bin directory and run ./stopServer.sh server_name
     
     For Example: /opt/IBM/WebSphere/AppServer/bin/startServer.sh server1
     
  6. Open default Web UI console at http://your-server:9060/ibm/console

## Setup PlantsByWebSphere
  
  1. Download file pbw.zip from this repository
  2. Unzip pbw.zip
  3. Deploy pbw-ear.ear
  4. Copy PLANTDB directory to WEBSPHERE-INSTALL-DIR/derby/databases
  5. Access the app from http://your-server:9080/PlantsByWebSphere/

## Install Transformation Advisor
  
  1. Download Transformation Advisor Installer from: https://www.ibm.com/account/reg/signup?formid=urx-38642
  2. Run the installer script locally: ./launchTransformationAdvisor.sh


  References:  
  Day Trader sample app can be found at:  
  http://geronimo.apache.org/GMOxDOC30/daytrader-a-more-complex-application.html  
  https://github.com/WASdev/sample.daytrader3  
  https://publib.boulder.ibm.com/wasce/V1.1.0/en/Tasks/Migrating/ToWebsphere.html  

