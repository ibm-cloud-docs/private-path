---

copyright:
  years: 2024, 2025
lastupdated: "2025-04-17"

keywords:

subcollection: private-path

content-type: release-note

---

{{site.data.keyword.attribute-definition-list}}

# Release notes for Private Path
{: #private-path-relnotes}

Check back regularly to see what's new with {{site.data.keyword.cloud}} Private Path service.
{: shortdesc}

### 10 April 2025
{: #privatepath-apr1025}
{: release-note}

Private path connectivity from IBM Cloud to on-premises locations (select availability)
:   Accounts with special approval can now connect a consumer service running in IBM Cloud to an on-premises provider service using an ALB as a member of a Private Path NLB pool. This allows you to target on-premises resources while maintaining a private path across IBM Cloud. For more information, see [Using an ALB with a Private Path NLB to host services outside a VPC](/docs/vpc?topic=vpc-private-path-service-intro&interface=ui#pps-use-case-5).

## 12 November 2024
{: #privatepath-nov1224}
{: release-note}

Private Path services for VPC
:   Private Path services are now generally available. Private Path services provide targeted and directional connectivity between VPCs and accounts, allowing only consumers to initiate connections to the provider's service endpoint. Explicit authorization gives providers full control of who can access their services.
A Private Path service requires a Private Path network load balancer to deploy a service on IBM Cloud, as well as a Virtual Private Endpoint (VPE) gateway for consumers to connect to the service.
{: note}

## 18 March 2024
{: #privatepath-march1824}
{: release-note}

Introducing the Private Path solution (Beta release)
:   The Private Path solution solves security, privacy and complexity problems for {{site.data.keyword.cloud}} consumers and providers who want to eliminate the risk of exposing their data on the public internet. The beta release of IBM Cloud Private Path services is only available to allowlisted users. Contact your IBM Support representative if you are interested in getting early access to this beta offering.
