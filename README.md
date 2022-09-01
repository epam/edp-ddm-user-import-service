# user-import-service

This service provides API for batch-import process: import/export files with user data, retrieving files info 

### Related components:
* `ddm-ceph-client` - service, which provides methods for working with storage

### Local development:
###### Prerequisites:
* Ceph/S3-like storage is configured and running

###### Configuration:
Check `src/main/resources/application-local.yaml` and replace if needed:
  * *-ceph properties with your ceph storage values

###### Steps:
1. (Optional) Package application into jar file with `mvn clean package`
2. Add `--spring.profiles.active=local` to application run arguments
3. Run application with your favourite IDE or via `java -jar ...` with jar file, created above

### License
user-import-service is Open Source software released under the Apache 2.0 license.
