
# Workflow Design Prompt

## Prompt

"Design an automated workflow for deploying a new version of a containerized web application to a Kubernetes cluster.

The workflow should be triggered when a new tag is pushed to the `main` branch of the Git repository.

The workflow should consist of the following steps:
1.  **Build Docker Image:** Build a new Docker image from the source code.
2.  **Push to Registry:** Push the Docker image to a container registry (e.g., Docker Hub, Harbor).
3.  **Update Kubernetes Manifests:** Update the Kubernetes deployment manifest with the new image tag.
4.  **Deploy to Staging:** Deploy the new version of the application to a staging environment.
5.  **Run E2E Tests:** Run end-to-end tests against the staging environment.
6.  **Deploy to Production:** If the tests pass, deploy the new version of the application to the production environment.

Please create a visual representation of the workflow using a diagram (e.g., a flowchart or a sequence diagram). You can use mermaidjs syntax for this."
