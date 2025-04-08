1. Add github-action.yaml as a workflow in your github repository
2. Create a client that has access to Zeebe API. Take note of the ClIENT_ID and CLIENT_SECRET
3. Create workflow secrets in the repository:

| Secret Name                           |                     Value |
|---------------------------------------|--------------------------:|
|ZEEBE_CLIENT_ID                    | CLIENT_ID from Identity       |
|ZEEBE_CLIENT_SECRET                | CLIENT_SECRET from Identity   |
|CLUSTER_REGION                     | your cluster region           |
|CLUSTER_ID                         | your cluster id               |
