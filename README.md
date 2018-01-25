
ArmClient login
ArmClient listmappings https://management.azure.com/subscriptions/<your subscription>/resourceGroups/<your group>/providers/Microsoft.Web/sites/<your site> 
(note the url format no trailing / or api-version)

In ArmClient:
ArmClient  get https://management.azure.com/subscriptions/<your subscription>/resourceGroups/<your group>/providers/Microsoft.Web/sites/<your site>/instances/<instance from previous results>/extensions/api/processes?api-version=2015-02-01
ArmClient delete https://management.azure.com/subscriptions/<your subscription>/resourceGroups/<your group>/providers/Microsoft.Web/sites/<your site>/instances/<instance from previous results>/extensions/api/processes/<process number>?api-version=2015-02-01
In resources.azure.com/raw:

## Get processes on a specific instance 
GET https://management.azure.com/subscriptions/<your subscription>/resourceGroups/<your group>/providers/Microsoft.Web/sites/<your site>/instances/<instance from previous results>/extensions/api/processes?api-version=2015-02-01
## Kill a specific process on a specific instance 
DELETE https://management.azure.com/subscriptions/<your subscription>/resourceGroups/<your group>/providers/Microsoft.Web/sites/<your site>/instances/<instance from previous results>/extensions/api/processes/<process number>?api-version=2015-02-01


 
