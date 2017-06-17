
Notes
=========

CoreMark Installation
----------------------

.. code-block::
  
  curl -L 'http://www.eembc.org/download/download.php?file_seq=924&user_seq=43844' > d
  tar xvzf d
  cd core*
  make PORT_DIR=linux64 XCFLAGS="-DMULTITHREAD=8 -DUSE_PTHREAD"


Docker for Hadoop 
------------------

Obtained from: https://github.com/sequenceiq/hadoop-docker

HADOOP
----------

.. code-block::

  cd $HADOOP_PREFIX
  bin/hadoop jar share/hadoop/mapreduce/hadoop-mapreduce-examples-2.7.1.jar pi 10 100
