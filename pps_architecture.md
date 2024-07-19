---

copyright:
  years:  2023, 2024
lastupdated: "2024-07-19"

keywords:

subcollection: private-path

---

{{site.data.keyword.attribute-definition-list}}

# Private Path service architecture
{: #private-path-service-architecture}

The beta release of IBM Cloud Private Path services is only available to allowlisted users. Contact your IBM Support representative if you are interested in getting early access to this beta offering.
{: beta}

A Private Path service provides private connectivity for {{site.data.keyword.cloud}} and third-party services. A Private Path service requires a Private Path network load balancer to deploy a service on IBM Cloud and a Virtual Private Endpoint (VPE) gateway for consumers to connect to the service. Traffic stays on the IBM backbone without crossing over the internet.
{: shortdesc}

## Private Path service architectural diagram
{: #private-path-service-architectural-diagram}

The following diagram illustrates the steps required for a Private Path service to connect Consumer and Provider services:

1. Provider creates the Private Path Network Load Balancer.
1. Provider creates a Private Path service resource and associates their service with the Private Path Network Load Balancer.
1. Consumer creates VPE Gateway that requests connectivity to the Private Path Service.
1. Provider approves the connectivity request, and connection is established.

![Private Path service architecture](images/private_path_use_case_1.svg "Private Path service architecture"){: caption="Figure 1. Private Path service architecture" caption-side="bottom"}

## Private Path service components
{: #private-path-service-components}

The following list describes common components included in a Private Path service:

Virtual Private Endpoint Gateway
:   Allows consumers to connect to a provider's service over a Private Path. To learn more, see [About virtual private endpoint gateways](/docs/vpc?topic=vpc-about-vpe).

Private Path service
:   Associates a provider's service with a Private Path network load balancer and to manage incoming connectivity requests. To learn more, see [About Private Path services](/docs/vpc?topic=vpc-private-path-service-intro&interface=ui).

Private Path connectivity
:   Links Provider's VPC and Consumer's VPC over private network paths using a [Virtual Private Endpoint Gateway](/docs/vpc?topic=vpc-about-vpe), eliminating the need for internet access.

Service providers
:   Includes the following:

    - Cloud Network Administrators from Consumer, ISV and IBM Cloud Services
    - Any industry, across all MZR geographies
    - IBM Cloud Services


Private Path network load balancer
:   Load balances traffic in a Private Path. Only receives requests across the IBM Cloud network. To learn more, see [About network load balancers](/docs/vpc?topic=vpc-network-load-balancers).

Transit Gateway
:   Connects VPCs within your network to enable them to share and access resources. To learn more, see [Accessing VPEs from an on-prem network using Direct Link or from another VPC using Transit Gateway](/vpc?topic=vpc-end-to-end-private-connectivity-vpe&interface=cli).

Direct Link
:   Directly connects to your IBM Cloud infrastructure without crossing over public internet and access your VPE Gateways for IBM Cloud Services. To learn more, see [Accessing VPEs from an on-prem network using Direct Link or from another VPC using Transit Gateway](/vpc?topic=vpc-end-to-end-private-connectivity-vpe&interface=cli).

Private DNS
:   Use a Private Domain Name System (DNS) to associate human friendly names with IP addresses. Private DNS zones are resolvable only on IBM Cloud, and only from explicitly permitted networks in an account. To learn more, see [Getting started with IBM Cloud DNS Services](/docs/dns-svcs?topic=dns-svcs-getting-started).


