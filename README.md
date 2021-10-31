
# upgrade pip
python -m pip install --upgrade pip

# install cassandta-driver
python -m pip install cassandra-driver

# install jupyter

python -m pip install jupyter

# launch jupyter notebook 
  jupyter notebook

  open the notebook "demo_cassandra_2022_esi-sba.ipynb"


#  start  the cassandra cluster
   docker-compose up -d

# Check that cassandra containers are starting
  docker ps

# Monitor cluster status
  docker exec cass nodetool status

# Check CQL is working
 docker exec -it cass   cqlsh  -e "describe keyspaces"
