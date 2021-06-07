ibm-cloud-inventory
========

#### IBM Cloud Infrastructure Inventory ####

This module provides an abstraction layer to inventory your cloud resources.

Supported services (and APIs):

Supported Regions
`us-west-1`

### Installation ###
```bash
npm install ibm-cloud-inventory
```

### Usage ###

```javascript
import IBMCloudInventory from 'ibm-cloud-inventory'

const config = {
  credentials: {
    accessKeyId: 'your_access_key',
    secretAccessKey: 'your_secret_key'
  },
  services: ['ec2', 'rds'],
  regions: ['us-west-2, us-east-1']
};

const oInventory = new IBMCloudInventory(config);
const oResources = oInventory.inventory();
```
