To run the test playbook(s) in this directory:

* Install and start Docker.
* Download the test shim (see .travis.yml file for the URL) into tests/test.sh:

wget -O tests/test.sh 

* Make the test shim executable: chmod +x tests/test.sh.
* Run (from the role root directory) distro=debian playbook=[playbook] ./tests/test.sh

If you don't want the container to be automatically deleted after the test playbook is run, 
add the following environment variables: `cleanup=false container_id=$(date +%s)`
