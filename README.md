terraform-docker
================
Docker container containing terraform. 
This image is based on hashicorps [terraform image](https://hub.docker.com/r/hashicorp/terraform/):light, with the entrypoint removed.
It is used for jenkins deployments where execution of docker run and terraform xxx don't hapen at the same time


Example Usage
-------------

```bash
docker run -it -v /path/to/credentials/.aws:/.aws -v $PWD/terraform/code/to/execute:/ checktheflow/terraform terraform apply
```

Links
-----

- [GitHub](https://github.com/checktheflow/terraform-docker)
- [terraform](https://www.terraform.io/)


License
-------

Released under the MIT License.
