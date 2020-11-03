---
title: 'Tutorial: Azure Active Directory single sign-on (SSO) integration with Hirebridge ATS | Microsoft Docs'
description: Learn how to configure single sign-on between Azure Active Directory and Hirebridge ATS.
services: active-directory
author: jeevansd
manager: CelesteDG
ms.reviewer: CelesteDG
ms.service: active-directory
ms.subservice: saas-app-tutorial
ms.workload: identity
ms.topic: tutorial
ms.date: 10/29/2020
ms.author: jeedes

---

# Tutorial: Azure Active Directory single sign-on (SSO) integration with Hirebridge ATS

In this tutorial, you'll learn how to integrate Hirebridge ATS with Azure Active Directory (Azure AD). When you integrate Hirebridge ATS with Azure AD, you can:

* Control in Azure AD who has access to Hirebridge ATS.
* Enable your users to be automatically signed-in to Hirebridge ATS with their Azure AD accounts.
* Manage your accounts in one central location - the Azure portal.

## Prerequisites

To get started, you need the following items:

* An Azure AD subscription. If you don't have a subscription, you can get a [free account](https://azure.microsoft.com/free/).
* Hirebridge ATS single sign-on (SSO) enabled subscription.

## Scenario description

In this tutorial, you configure and test Azure AD SSO in a test environment.

* Hirebridge ATS supports **IDP** initiated SSO


## Adding Hirebridge ATS from the gallery

To configure the integration of Hirebridge ATS into Azure AD, you need to add Hirebridge ATS from the gallery to your list of managed SaaS apps.

1. Sign in to the Azure portal using either a work or school account, or a personal Microsoft account.
1. On the left navigation pane, select the **Azure Active Directory** service.
1. Navigate to **Enterprise Applications** and then select **All Applications**.
1. To add new application, select **New application**.
1. In the **Add from the gallery** section, type **Hirebridge ATS** in the search box.
1. Select **Hirebridge ATS** from results panel and then add the app. Wait a few seconds while the app is added to your tenant.


## Configure and test Azure AD SSO for Hirebridge ATS

Configure and test Azure AD SSO with Hirebridge ATS using a test user called **B.Simon**. For SSO to work, you need to establish a link relationship between an Azure AD user and the related user in Hirebridge ATS.

To configure and test Azure AD SSO with Hirebridge ATS, perform the following steps:

1. **[Configure Azure AD SSO](#configure-azure-ad-sso)** - to enable your users to use this feature.
1. **[Assign an Azure AD user](#assign-an-azure-ad-user)** - to enable one of your users to use Azure AD single sign-on.
1. **[Configure Hirebridge ATS SSO](#configure-hirebridge-ats-sso)** - to configure the single sign-on settings on application side.
1. **[Test SSO](#test-sso)** - to verify whether the configuration works.

## Configure Azure AD SSO

Follow these steps to enable Azure AD SSO in the Azure portal.

1. In the Azure portal, on the **Hirebridge ATS** application integration page, find the **Manage** section and select **single sign-on**.
1. On the **Select a single sign-on method** page, select **SAML**.
1. On the **Set up single sign-on with SAML** page, click the edit/pen icon for **Basic SAML Configuration** to edit the settings.

   ![Edit Basic SAML Configuration](common/edit-urls.png)

1. On the **Basic SAML Configuration** section, the application is pre-configured and the necessary URLs are already pre-populated with Azure. The user needs to save the configuration by clicking the **Save** button.

1. On the **Set up single sign-on with SAML** page, in the **SAML Signing Certificate** section,  click **Add a certificate**.

	![Add certficate link](common/add-saml-certificate.png)

1. On the **SAML Signing Certificate** popup, click **New Certificate** and then click **Save**. When saving is complete, close the popup by clicking the **X** in the top-right corner.

	![Create certificate link](common/new-saml-certificate.png)

1. In the **SAML Signing Certificate** section, find the **App Federation Metadata Url** and copy it,

	![Copy Mtadata Url link](common/copy-metadataurl.png)

### Assign an Azure AD user

In this section, you'll enable one of your users to use Azure single sign-on by granting access to Hirebridge ATS.

1. In the Azure portal, select **Enterprise Applications**, and then select **All applications**.
1. In the applications list, select **Hirebridge ATS**.
1. In the app's overview page, find the **Manage** section and select **Users and groups**.
1. Select **Add user**, then select **Users and groups** in the **Add Assignment** dialog.
1. In the **Users and groups** dialog, select the user you would like to test from the Users list, then click the **Select** button at the bottom of the screen. This user must exist in the Hirebridge system with the same email address as their primary Azure AD email.
1. If you are expecting a role to be assigned to the users, you can select it from the **Select a role** dropdown. If no role has been set up for this app, you see "Default Access" role selected.
1. In the **Add Assignment** dialog, click the **Assign** button.

## Configure Hirebridge ATS SSO

To configure single sign-on on **Hirebridge ATS** side, you need to be an administrator within the Hirebridge system. 

1. In the **Administration Control Panel**, in the **Users/Permissions** section, click on **Single Sign-On Configuration**  
1. Click the **Import Metadata** button at the bottom of the page.
1. Paste the metadata URL that you copied earlier into the space provided and click **Import**.

The certificate and Entity ID will be extracted from the metadata and saved to your configuration. If you have any issues, contact the [Hirebridge ATS support team](mailto:support@hirebridge.com).

## Test SSO 

In this section, you test your Azure AD single sign-on configuration with following options.

1. Click on Test this application in Azure portal and you should be automatically signed in to the Hirebridge ATS for which you set up the SSO

1. You can use Microsoft Access Panel. When you click the Hirebridge ATS tile in the Access Panel, you should be automatically signed in to the Hirebridge ATS for which you set up the SSO. For more information about the Access Panel, see [Introduction to the Access Panel](https://docs.microsoft.com/azure/active-directory/active-directory-saas-access-panel-introduction).

## Next steps

Once you configure Hirebridge ATS you can enforce session control, which protects exfiltration and infiltration of your organization’s sensitive data in real time. Session control extends from Conditional Access. [Learn how to enforce session control with Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/proxy-deployment-any-app).


