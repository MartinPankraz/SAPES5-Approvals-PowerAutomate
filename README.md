# SAPES5-Approvals-PowerAutomate
This repos contains the dev content for my integration prototype between SAP ES5 and PowerAutomate

- GetPurchaseOrderApprovals: Teams integration with adaptive card
- GetPurchaseOrderApprovalsInO365: Outlook integration with actionable messages
- ProcessActionableMessage: endpoint for actions from card in Outlook
- PreloadPOFromSAPES5: helper flow to store purchase order approvals in Azure to overcome latency restriction (request to ES5 takes longer than allowed 2secs for auto-invoke function on actionable messages)
- GetPreloadedPOFromSAPES5: helper flow to work with pre-loaded purchase order ids from SAP ES5.

![Overview_Image](https://github.com/MartinPankraz/SAPES5-Approvals-PowerAutomate/blob/master/pictures/actionable-messages-overview.png)

Please note that the helper flows are Azure Logic Apps. I did that for internal reasons and policy regulations. In your environment I would recommend to stick either to PowerAutomate or Logic Apps only. Not for technical but administrative reasons.

Please find the associated blog on the SAP community here: https://blogs.sap.com/2020/09/18/last-action-hero-with-adaptive-cards-for-cloud-demo-system-es5

I added placeholders "<<<>>>" on the definitions files for you to configure with your own values. However it might be easier to just copy the relevant configurations and re-create the "hull" yourself.
