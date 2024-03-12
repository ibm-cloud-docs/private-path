---

copyright:
  years:  2023
lastupdated: "2023-12-19"

keywords:

subcollection: private-path

---

{{site.data.keyword.attribute-definition-list}}

# Private Path service roles and responsibilities
{: #private-path-service-roles-and-responsibilities}

The beta release of IBM Cloud Private Path services is only available to allowlisted users. Contact your IBM Support representative if you are interested in getting early access to this beta offering.
{: beta}

As a service provider, you are responsible to manage your consumer account IDs. Tracking or validating account IDs is currently not supported. The responsibility of managing, approving, and revoking consumer account IDs lies entirely with you as the service provider. For more information, see [Responsibilities for Managing Consumer Account IDs](/docs/vpc?topic=vpc-pps-consumer-account-id-responsibilities&interface=ui).
{: beta}

Private Path service is an orchestration service between a Provider and Consumer. As you consume IBM Cloud services, be aware of your roles and responsibilities. For more information, see [Understanding your responsibilities when using Virtual Private Cloud](/docs/vpc?topic=vpc-responsibilities-vpc){: external}.
{: shortdesc}

The following table describes the roles and responsibilities shared betwen IBM Cloud and the Provider in a Private Path service.


## Incident and operations management
{: #incident-and-ops-responsibilities}

| Task | {{site.data.keyword.cloud_notm}} Responsibilities | Provider Responsibilities |
|----------|-----------------------|--------|
| Monitoring | {{site.data.keyword.cloud_notm}} is responsible for providing tooling for monitoring your activities and health services. | The Client is responsible for integrating with the [{{site.data.keyword.monitoringfull}}](/docs/monitoring?topic=monitoring-platform_metrics_enabling) including Sysdig Monitor, [{{site.data.keyword.at_full}}](/docs/cloud-databases?topic=cloud-databases-activity-tracker), or [{{site.data.keyword.loganalysisfull}}](/docs/cloud-databases?topic=cloud-databases-logging). |
| High Availability | {{site.data.keyword.cloud_notm}}  is responsible for providing infrastructure to meet client needs for high availabiity. | The Client is responsible for deploying their application across multiple zones and provisioning their load balancer across multiple zones to prevent single points of failure. |
| Performance | {{site.data.keyword.cloud_notm}} is responsible for infrastructure performance. | The Client is responsible for application performance. |
{: caption="Table 1. Responsibilities for incident and operations" caption-side="top"}

## Change management
{: #change-management-responsibilities}

| Task | {{site.data.keyword.IBM_notm}} Responsibilities | Provider Responsibilities |
|----------|-----------------------|--------|
|Scaling| IBM Cloud is responsible for scaling infrastructure to meet client requests. | The Client is responsible for choosing, monitoring, and scaling disk, memory, and CPU core allocation for their applications by using the UI or API. |
| Version management | IBM Cloud is responsible for updating infrastructure. | The Client is responsible for updating their applications as required. |
{: caption="Table 2. Responsibilities for change management" caption-side="top"}

## Security and regulation compliance
{: #security-responsibilities}

| Task | {{site.data.keyword.IBM_notm}} Responsibilities | Provider Responsibilities |
|----------|-----------------------|--------|
| Encryption | {{site.data.keyword.cloud_notm}} encryption with respect to Private Path service is not applicable. | The Client is responsible for choosing and managing appropriate additional security features for their application. |
| Security | {{site.data.keyword.cloud_notm}} is responsible for infrastructure security. | The Client is responsible for their application security. |
| Compliance | {{site.data.keyword.cloud_notm}} is responsible for infrastructure compliance. | The Client is responsible for their application compliance. |
{: caption="Table 3. Responsibilities for security and regulation compliance" caption-side="top"}

## Disaster recovery
{: #disaster-recovery-responsibilities}

| Task | {{site.data.keyword.IBM_notm}} Responsibilities | Provider Responsibilities |
|----------|-----------------------|--------|
|Backups and restore| {{site.data.keyword.cloud_notm}} is responsible for infrastructure backup and restore. | The Client is responsible for their application backup and restore. |
{: caption="Table 4. Responsibilities for disaster recovery" caption-side="top"}
