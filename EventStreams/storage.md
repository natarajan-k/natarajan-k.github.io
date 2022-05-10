# Changing StorageClass for an existing EventStream

This document will list out the steps for changing the StorageClass of a PVC used by EventStreams. Customers may want to chnage their storage attached to OpenShift and hence may have to move the EventStreams data to the new storage. This article explains how to achieve this. 

## Pre-requsites
1. You should have a working EventStreams pointing to an exisating StorageClass. 
2. You have a new storage attached to OpenShift and a new StorageClass created.
3. All topics must have at least 3 replicas. 
4. Please note that data in topics without replicas will be lost.

