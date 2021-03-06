---
layout: "enterprise2"
page_title: "Private Terraform Enterprise Configuration"
sidebar_current: "docs-enterprise2-private-config"
---

# Private Terraform Enterprise Configuration

After you have completed the installation process you will need to create an
admin user. When the admin user creation has been completed you will
be able to create your first organizations and users and enable the enterprise
features for those accounts.

~> **Note:** If you are performing an upgrade or restore for an existing
installation you _do not_ need to follow these steps. If your upgraded or
restored installation does not function without the steps below then it was not
correctly restored from backup. Please contact HashiCorp for help.

## System Configuration

In all examples below, be sure to replace "`<TFE HOSTNAME>`" with the hostname
of your Private Terraform Enterprise instance.

Navigate to `https://<TFE HOSTNAME>:8800/` in your browser. You will
be presented with the installer dashboard:

![PTFE Installer Dashboard](./assets/post-install-repl-console.png)

### Creating an Administrator

After clicking on the "Open", right below the "Stop Now" button, you will
be brought to a page asking you to create the first PTFE administrator account.
You will be able to create additional administrators once you log in.

![New admin dialog](./assets/create-an-account.png)

### Creating an organization

The next step will create the first organization.

![Create a new organization](./assets/create-organization.png)

After this is done, you can either continue with the creation of a new workspace,
choose to configure other aspects of PTFE, or add more users.

## Success!

You have successfully configured the installation and configuration steps that
are specific to Private Terraform Enterprise! You can now configure SMTP
(`https://<TFE HOSTNAME>/app/admin/smtp/`), Twilio (`https://<TFE HOSTNAME>/app/admin/twillio`),
SAML (`https://<TFE HOSTNAME>/app/admin/saml`), or head to the [Getting Started](/docs/enterprise/getting-started/index.html)
section to start using the software.
