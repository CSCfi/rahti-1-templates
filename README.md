# Rahti 1 templates (Legacy templates)

You can find in this repo some of the Rahti 1 templates.  

**These templates won't be updated by CSC. We strongly recommend to use the new [Helm Charts](https://github.com/CSCfi/helm-charts) developed by CSC to deploy your applications on Rahti 2.**
## How to use them?

First, clone the repository on your local computer.  
Navigate to the cloned folder and you can apply the template with the [oc](https://docs.csc.fi/cloud/rahti2/usage/cli/) command:

  ```sh
  oc process -f {name_of_the_template} | oc apply -f -
  ```

If some parameters are needed, you can specific them:

  ```sh
  oc process -f {name_of_the_template} -p {parameter_name}={value} ... | oc apply -f -
  ```

To delete all the resources, you can use this command:

  ```sh
  oc process -f {name_of_the_template} | oc delete -f -
  ```
  