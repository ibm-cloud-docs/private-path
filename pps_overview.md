---

copyright:
  years:  2023, 2024
lastupdated: "2024-10-24"

keywords:

subcollection: private-path

---

{{site.data.keyword.attribute-definition-list}}

# About Private Path
{: #overview}

The Private Path solution solves security, privacy and complexity problems. Through Private Path, providers can deliver their services over the IBM Cloud private network backbone, ensuring secure and private interactions for consumers. Providers can offer their services to IBM Cloud customers over Private Path using the IBM Cloud infrastructure. Private Path components are used when connecting to IBM Cloud services, and can now be used for third-party applications and services.

The Private Path solution has the following advantages:

Increased security and privacy
:   Private Path allows targeted and directional connectivity between VPCs and accounts, allowing only consumers to initiate connections to the provider's service endpoint. 

Granular control
:   Explicit authorization gives Providers full control over who can access their services

Scaling out managed services
:   Point-to-point connectivity, with no other shared resource dependencies between consumer and producer VPC networks, simplifies deployment and enables providers to easily scale managed services.

Decreased complexity
:   Simplify cloud network management and consume services directly in virtual networks without needing complex setups. Set up access policy enforcement and quickly expose and consume services across different networks and organizations.
 
Line rate performance
:   Stateless load balancing enables bypassing intermediate hops resulting in optimal performance.

High-Availability
:   Zonal resilience for PPNLB ensuring regional fault-tolerance and high-availability.

The Private Path solution incorporates various products that IBM Cloud customers are already familiar with, such as VPC and network load balancers. It also incorporates any configured Virtual Private Endpoint (VPE) gateways and DNS Services, ensuring that the entire point-to-point data path is private across IBM Cloud. 

![Private Path service overview](images/private_path_overview.svg "Private Path service overview"){: caption="A consumer VPE using a Private Path to connect to a service" caption-side="bottom"}

To use IBM Cloud Private Path, you must first have an IBM Cloud account. To learn more, see [Setting up your IBM Cloud account](/docs/account?topic=account-account-getting-started){: external}.
{: note}

## Private Path overview video
{: #private-path-overview-video}

Forthcoming

## Next steps
{: #private-path-next-steps}

The following links provide additional information about the Private Path solution:

- [Private Path service architecture](/docs/private-path?topic=private-path-private-path-service-architecture){: external}
- [About Private Path services](/docs/vpc?topic=vpc-private-path-service-intro&interface=ui){: external}
- [Creating a Private Path network load balancer](/docs/vpc?topic=vpc-ppnlb-ui-creating-private-path-network-load-balancer&interface=ui){: external}
- [Creating a Private Path service](/docs/vpc?topic=vpc-private-path-service-about&interface=ui){: external}
