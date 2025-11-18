# Ecxports the Genie Space Metadata

To get the CLIENT_ID and CLIENT_SECRET values do the following:
1. If the PAT token is expired (typically after 90 days) then generate a new one for the workspace
2. Create the scope if not already done using CLI
  * `databricks secrets create-scope amitabh_arora_scope`

3. use the following CLI to update the client id and secret of PAT token is obsolete
  * `databricks secrets put-secret amitabh_arora_scope e2-demo-field-eng --string-value "<workspace-pat-token>"`
