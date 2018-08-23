## Geonode / Geoserver External Data Directory

This directory contains all data (shp files, rasters, etc.) that has to be made avilable in the geonode / geoserver containers. It is [bind-mounted](https://docs.docker.com/storage/bind-mounts/) into the geoserver and geonode docker containers, so all files copied into this directory are immediately available in these docker containers.

Please note, that the *ext_data* directory is different from the *geoserver_data* which a a) mainly used to store the GeoServer configuration and b) a *named volume* from a dedicated 'data container' as explained [here](https://github.com/GeoNode/data-docker#data-volumes)


See also [Access the GeoServer Data Directory](https://github.com/clarity-h2020/docker-geonode/issues/4)