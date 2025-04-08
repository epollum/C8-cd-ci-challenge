1. Add github-action.yaml as a workflow in your github repository
2. Create a client that has access to Zeebe API. Take note of the ClIENT_ID and CLIENT_SECRET
![image](https://github.com/user-attachments/assets/02a5a532-d96e-490f-a0fd-8f41bd8e11b1)

4. Create action secrets in the repository:
![image](https://github.com/user-attachments/assets/725dab09-c637-4b86-b4bd-7fb96cf2a57b)


| Secret Name                       |                         Value |
|-----------------------------------|------------------------------:|
|ZEEBE_CLIENT_ID                    | CLIENT_ID from Identity       |
|ZEEBE_CLIENT_SECRET                | CLIENT_SECRET from Identity   |
|CLUSTER_REGION (SaaS only)         | your cluster region           |
|CLUSTER_ID (SaaS only)             | your cluster id               |
|ZEEBE_GATEWAY_URL (SM only)        | url of your zeebe gateway     |


For SM, replace the URL in the *Deploy to Zeebe* with _curl -X POST "https://${{ secrets.ZEEBE_GATEWAY_URL }}/v2/deployments"
