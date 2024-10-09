---

copyright:
  years:  2023, 2024
lastupdated: "2024-10-09"

keywords:

subcollection: private-path

---

{{site.data.keyword.attribute-definition-list}}

# Private Path architecture
{: #private-path-service-architecture}

The beta release of {{site.data.keyword.cloud}} Private Path services is only available to allowlisted users. Contact your IBM Support representative if you are interested in getting early access to this beta offering.
{: beta}

A Private Path service provides private connectivity for IBM Cloud and third-party services. A Private Path service requires a Private Path network load balancer (NLB) to deploy a service on IBM Cloud and a Virtual Private Endpoint (VPE) gateway for consumers to connect to the service.
{: shortdesc}

Figure 1 illustrates the steps required for a Private Path service to connect consumers to provider' services and applications:

1. The provider creates a Private Path NLB.
1. The provider creates a Private Path service and associates their service with the Private Path NLB.
1. The consumer creates a VPE gateway that requests connectivity to the Private Path service.
1. The provider approves the connectivity request and establishes the connection.

![Private Path service architecture](images/private_path_use_case_1.svg "Private Path service architecture"){: caption="Private Path service architecture" caption-side="bottom"}

## Private Path service components
{: #private-path-service-components}

The following list describes common components included in a Private Path service:

VPE gateway
:   Allows consumers to connect to a provider's service using the service's cloud resource name (CRN). To learn more, see [About virtual private endpoint gateways](/docs/vpc?topic=vpc-about-vpe).

Private Path service
:   Associates a provider's service with a Private Path NLB to manage incoming connectivity requests. To learn more, see [About Private Path services](/docs/vpc?topic=vpc-private-path-service-intro&interface=ui).

Private Path NLB
:   Load balances traffic in a Private Path service, only receiving requests across the IBM Cloud network. To learn more, see [About network load balancers](/docs/vpc?topic=vpc-network-load-balancers).

DNS Services
:   Uses a private Domain Name System (DNS) to associate human friendly names with IP addresses. Private DNS zones are resolvable only on IBM Cloud, and only from explicitly permitted networks in an account. To learn more, see [Getting started with IBM Cloud DNS Services](/docs/dns-svcs?topic=dns-svcs-getting-started).
