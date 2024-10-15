---

copyright:
  years:  2023, 2024
lastupdated: "2024-10-09"

keywords:

subcollection: private-path

---

{{site.data.keyword.attribute-definition-list}}

# About Private Path
{: #overview}

The Private Path solution solves security, privacy and complexity problems. Through Private Path, providers can deliver their services over the IBM Cloud private network backbone, ensuring secure and private interactions for consumers. Providers can offer their services to IBM Cloud customers over Private Path using the IBM Cloud infrastructure. Private Path components are used when connecting to IBM Cloud services, and can now be used for third-party applications and services.

The Private Path solution has the following advantages:

Increased security and privacy
:   Securely connect to services and applications deployed on IBM Cloud. Avoid exposure of data to the internet by accessing services directly over the IBM Cloud backbone.

Decreased complexity
:   Simplify cloud network management and consume services directly in virtual networks without needing complex setups. Set up policy enforcement and quickly expose and consume services across different networks and organizations.

Point-to-point connectivity
:   Private Path allows targeted and directional connectivity between VPCs and accounts, allowing only consumers to initiate connections to the provider; the provider cannot initiate connections to consumer' VPCs. 

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
