---

copyright:
  years:  2023, 2024
lastupdated: "2024-10-09"

keywords:

subcollection: private-path

---

{{site.data.keyword.attribute-definition-list}}

# Private Path service roles and responsibilities
{: #private-path-service-roles-and-responsibilities}

The beta release of IBM Cloud Private Path services is only available to allowlisted users. Contact your IBM Support representative if you are interested in getting early access to this beta offering.
{: beta}

Private Path service is an orchestration service. The roles and responsibilities for Private Path connectivity are shared between the Provider and Consumer, not IBM Cloud. 
{: note}

As you consume IBM Cloud services, be aware of your roles and responsibilities. For more information, see [Understanding your responsibilities when using Virtual Private Cloud](/docs/vpc?topic=vpc-responsibilities-vpc).

The following table describes the roles and responsibilities shared betwen the Provider and Consumer in a Private Path service.

| Task | Provider | Consumer |
|----|----|----|
| Configure your Private Path network load balancer (NLB) |  Use the same VPC region for the Private Path NLB and the Private Path service. Create at least one subnet in your selected VPC. You should also create your virtual server instances prior to [creating a Private Path NLB](/docs/vpc?topic=vpc-ppnlb-ui-creating-private-path-network-load-balancer&interface=ui) to ensure it is fully operational. | None |
| Verify your service | Always [verify connectivity to your Private Path service](/docs/vpc?topic=vpc-pps-verify&interface=ui) before you publish. This action cannot be undone. | None |
| Publish your Private Path service | After you verify successful connectivity to your Private Path service, you should then [publish your service](/docs/vpc?topic=vpc-pps-activating&interface=ui) for deployment to consumers. | None |
| Create a Virtual Private Endpoint gateway | None | You must [create an endpoint gateway](/docs/vpc?topic=vpc-ordering-endpoint-gateway&interface=ui) to connect to a Private Path service. |
| Request connection to a service | None | Use the connection information communicated by your service provider to request access to their service. Check your IBM Cloud account for updates on your request's approval or denial. |
| Permit connection to a service | Either configure an access policy or manually [review connection requests](/docs/vpc?topic=vpc-pps-ui-reviewing&interface=ui) for your Private Path service. | None |
| Provide connection information | [Communicate connection information to your consumers](/docs/vpc?topic=vpc-pps-ui-communicate), such as the CRN, applicable ports, and information on how to create a VPE gateway, so that they can connect to your service. | None |
{: caption="Roles and Responsibilities" caption-side="bottom"}
