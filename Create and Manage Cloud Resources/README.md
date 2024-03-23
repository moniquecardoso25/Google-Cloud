# Chalenge Scenario - Lab

## Credits
- Google Skill Boost - Quicklabs
- Challenge lab from Badge: Create and Manage Cloud Resources


You've taken on the role of a Junior Cloud Engineer at Jooli, where your responsibilities include managing the company's infrastructure. This involves tasks like provisioning resources for projects.

In order to excel in this role, you're expected to possess the necessary skills and knowledge. Detailed, step-by-step guides won't be provided, so you should be adept at carrying out these tasks independently.

Jooli company has set specific standards that you should adhere to:

1. Create all resources in the default region or zone, unless instructed otherwise.
2. Follow the naming convention of team-resource. For instance, an instance could be named ***nucleus-webserver1***.
3. Opt for cost-effective resource sizes. Remember that projects are under constant monitoring, and using excessive resources may lead to the termination of the entire project (and potentially your own role). To avoid this, plan your resource allocation thoughtfully. As a guideline, unless otherwise specified, use ***e2-micro*** for small Linux VMs, and opt for e2-medium for applications like Windows or Kubernetes nodes.

## Task 1. Create a project jumphost instance

Requirements:
- Name the instance Instance name.
- Use an e2-micro machine type.
- Use the default image type (Debian Linux).

## Task 2. Create a Kubernetes service cluster

The team is building an application that will use a service running on Kubernetes. You need to:

- Create a zonal cluster using <filled in at lab start>.
- Use the Docker container hello-app (gcr.io/google-samples/hello-app:2.0) as a placeholder; the team will replace the container with their own work later.
- Expose the app on port App port number.

## Task 3. Set up an HTTP load balancer
You will serve the site via nginx web servers, but you want to ensure that the environment is fault-tolerant. Create an HTTP load balancer with a managed instance group of 2 nginx web servers. Use the following code to configure the web servers; the team will replace this with their own configuration later.

You need to:

- Create an instance template.
- Create a target pool.
- Create a managed instance group.
- Create a firewall rule named as Firewall rule to allow traffic (80/tcp).
- Create a health check.
- Create a backend service, and attach the managed instance group with named port (http:80).
- Create a URL map, and target the HTTP proxy to route requests to your URL map.
- Create a forwarding rule.
