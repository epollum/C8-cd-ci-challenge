1. Add github-action.yaml as a workflow in your github repository
2. Create a client that has access to Zeebe API. Take note of the ClIENT_ID and CLIENT_SECRET
3. Create workflow secrets in the repository:

| Secret Name                       |                         Value |
|-----------------------------------|------------------------------:|
|ZEEBE_CLIENT_ID                    | CLIENT_ID from Identity       |
|ZEEBE_CLIENT_SECRET                | CLIENT_SECRET from Identity   |
|CLUSTER_REGION (SaaS only)         | your cluster region           |
|CLUSTER_ID (SaaS only)             | your cluster id               |
|ZEEBE_GATEWAY_URL (SM only)        | url of your zeebe gateway     |


For SM, replace the URL in the *Deploy to Zeebe* with _curl -X POST "https://${{ secrets.ZEEBE_GATEWAY_URL }}/v2/deployments"
