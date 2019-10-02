# Devops/GIS engineer - Technical task

Thanks for applying to work at FATMAP. We have developed this task for you to work on in your own time so that we can see how you approach tasks and as a discussion point going forwards.

## The Task

We would like you to do the following:

### 1. Create GeoJSON validating server component
The component should accept a `POST` request containing GeoJSON, validate the structure of the GeoJSON (either locally or by connecting to and using an online GeoJSON validation service), and return a meaningful JSON response.

The `aoi.geojson` file can be used to test the POST endpoint.

### 2. Dockerise the component
Create `Dockerfile` and `docker-compose.yml` files for the component you have created in Step 1. Running `docker-compose up` should expose the service via a port on your local machine: you should be able to `POST` GeoJSON to the server via this port.

### 3. Deploy the component to a local Kubernetes cluster
Deploy the component to a Kubernetes instance that you have running on your local machine.

You should be able to:

* Access the service from outside of the cluster (i.e. be able to `POST` and receive GeoJSON from your local machine).
* Be able to scale up and down the number of instances of the component.

### 4. Document the deployment process
Please provide all the necessary files along with accompanying technical documentation on how to replicate the setup and deploy the cluster on a local machine.  

All files should be committed to a publically accessible git repository.
