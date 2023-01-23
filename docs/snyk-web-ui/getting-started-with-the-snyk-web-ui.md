---
description: Introduction to what you can do in the Snyk Web UI
---

# Exploring the Snyk Web UI

No matter how you use Snyk, you can use the Snyk Web UI to connect your source code management (SCM) repositories, container registries, and applications. If you haven't already, go to the [Snyk Web UI](https://app.snyk.io/login) and [create an account](../getting-started/quickstart/create-a-snyk-account.md).

After you connect, you can import your repositories and projects for Snyk to scan, monitor, and fix vulnerabilities in your source code.

## Set up the Snyk Web UI

When you log in to an existing account, the Web UI opens to the [Dashboard](getting-started-with-the-snyk-web-ui.md#dashboard). Initially a wizard can guide you through setup steps:

1. Identifying where the code you want to monitor in Snyk is located.
2. Defining which projects within your code you want Snyk to scan.
3. Connecting Snyk to the relevant projects to scan them.
4. Reviewing the results of your Snyk scan.

{% hint style="info" %}
If you are signing in to a paid account, you must also select the relevant [Organization](../snyk-admin/managing-groups-and-organizations/whats-a-snyk-organization.md) after you log in to Snyk.
{% endhint %}

In the following example, the Snyk dashboard for an Enterprise account shows pending tasks, vulnerable projects, and current security and license issues.

<figure><img src="../.gitbook/assets/web_ui-landing_02oct2022.png" alt="Snyk dashboard for an Enterprise account"><figcaption><p>Snyk dashboard for an Enterprise account</p></figcaption></figure>

## What can I do on the Web UI pages?

* [Explore the dashboard](getting-started-with-the-snyk-web-ui.md#dashboard)
* [Investigate reports](getting-started-with-the-snyk-web-ui.md#reports)
* [Manage Projects](getting-started-with-the-snyk-web-ui.md#manage-your-projects)
* [Manage integrations](getting-started-with-the-snyk-web-ui.md#manage-your-integrations)
* [Manage Group or Organization members](getting-started-with-the-snyk-web-ui.md#manage-organization-or-group-members)
* [View Snyk updates](getting-started-with-the-snyk-web-ui.md#view-product-updates)
* [Get help](getting-started-with-the-snyk-web-ui.md#view-helpful-resources)
* [Manage my user account](getting-started-with-the-snyk-web-ui.md#manage-account-preferences-and-settings)

## Dashboard

On the Dashboard, you can view your pending tasks and vulnerable projects, invite team members, and add new Projects. You can also use the Add Project link to add a new Project.

The **Pending tasks** section shows the next chores to be handled for the Projects in a Snyk Organization. This information includes:

* Pull Requests (PRs) that can be raised to fix vulnerabilities in some of the most vulnerable projects.
* PRs that have already been raised by or through Snyk and are open and awaiting review.

Currently, Snyk tracks and flags PRs in GitHub, GitHub Enterprise, and Bitbucket Cloud only, and only for the top-most vulnerable projects. If you use another SCM, **Pending tasks** shows only PRs that can be raised, and not PRs that have already been raised.

<figure><img src="../.gitbook/assets/image (109).png" alt="Pending tasks and Vulnerable Projects listed on the Dashboard"><figcaption><p>Pending tasks and Vulnerable Projects listed on the Dashboard</p></figcaption></figure>

You can use the **Add project** link on the dashboard to add a Project. Select the way you want to add the Project from the dropdown.

Use the links for Projects on the dashboard to explore and manage the metadata, retest, and fix options for the Targetfiles in your Projects. Each link opens a Project details page where you can view the Project **Overview**, or switch to the **History** and **Settings** tabs.

* For Projects with the **Fix vulnerabilities** link, use the link to view Project details with an option to **Open a Fix PR.** Use this option to open a fix PR to implement the upgrades and patches in GitHub that address the issues.
* For Projects with a **View PR** link, use the link to open and view the Snyk-generated PR fixes in GitHub.

<figure><img src="../.gitbook/assets/dockerfile_fix_vulnerabilities (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).gif" alt="Demo, add project and Project details tabs"><figcaption><p>Demo, add project and Project details tabs</p></figcaption></figure>

## **Reports**

You can view [reports](../features/snyk-reports/) to gain visibility and insights into the state of all your Projects, vulnerabilities, and license issues.

{% hint style="info" %}
**Feature availability**\
The **Reports** tab is fully enabled for Enterprise plans.
{% endhint %}

<figure><img src="../.gitbook/assets/reports.gif" alt="Demo of viewing reports, filters, and summary filters"><figcaption><p>Demo of viewing reports, filters, and summary filters</p></figcaption></figure>

## **Manage your** **Projects**

Select the **Projects** link in the navigation on the dashboard to open the **Projects** listing page where you can:

* Add a Project. Select the way you want to add the Project from the dropdown.
* Filter, group, and sort your Projects.
* View tips and the latest import log for your Projects.
* Select the link for each Project to view the Project details page with a summary and Issue information.
* Use the plus icon and add a Target from a custom location when Projects are grouped by Target. This allows for grouping projects in another Target in the list.
* Use the settings icon on the ungrouped **Projects** listing or the **Settings** tab on the Project detail page to configure General and GitHub integration settings for notifications, Project testing, and pull request (PR) frequency. You can also look up the unique Project ID and deactivate or delete a project on the Settings tab.
* View the Project history on the **History** tab.

<figure><img src="../.gitbook/assets/Project listing add projects.gif" alt="Options on the Projets listing page"><figcaption><p>Options on the Projets listing page</p></figcaption></figure>

## **Manage your** **Integrations**

Select **Integrations** from the navigation on the dashboard to open the [Integrations](../integrations/) page where you can do the following:

* View the supported environments that can connect to Snyk for vulnerability monitoring.
* Manage [Slack](https://docs.snyk.io/integrations/notifications-ticketing-system-integrations/slack-integration) and [Jira](https://docs.snyk.io/integrations/notifications-ticketing-system-integrations/jira) integrations.
* Learn about the [Vulnerability management tools](https://docs.snyk.io/integrations/vulnerability-management-tools).

<figure><img src="../.gitbook/assets/image (157) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Integrations page"><figcaption><p>Integrations page</p></figcaption></figure>

## Manage Organization or Group members

Select **Members** from the navigation on the dashboard to view and manage users, roles, and how users authenticate in your Snyk [Organization](../snyk-admin/managing-users-and-permissions/manage-users-in-your-organizations.md) or [Group](../user-and-group-management/managing-users-and-permissions/manage-users-in-your-organizations-1.md).

{% hint style="info" %}
You must be assigned the [required Admin roles and permissions](../snyk-admin/managing-users-and-permissions/managing-permissions.md) to make changes in the **Members** tab.
{% endhint %}

## Snyk Organization or Group Settings

Use the <img src="../.gitbook/assets/cog_icon.png" alt="" data-size="line"> menus to view and manage your Organization (team) or Group (company-wide) settings.

<figure><img src="../.gitbook/assets/image (145) (1) (1) (1) (1) (1) (1) (1).png" alt="Group and Organization settings"><figcaption><p>Group and Organization settings</p></figcaption></figure>

See [Managing settings](../snyk-admin/managing-settings/) for more details.

## View product updates

Select **Help** in the navigation on the dashboard and then select **Product updates** to visit [snyk.io updates](https://updates.snyk.io/).

## View helpful resources

Select **Help** in the navigation on the dashboard and then select an option to view resources with information about Snyk.

## Manage account preferences and settings

Select your **name** in the navigation on the dashboard and then **Account settings** to open your [account settings](https://app.snyk.io/account) page where you can view and configure your user account settings and your notification and sharing preferences.

You have access to the following information and options in the in the Account Settings:

* View and manage your API token (or the Auth Token for free accounts).
* View the list of your Authorized Applications.
* Set your Preferred Organization.
* Delete your account.
* Manage your notification preferences for Email Notifications, Issue email alerts, the Weekly report, Usage alerts, Report status, and Marketing & Sales Communications.
* Share a Snyk referral link with your friends.

<figure><img src="../.gitbook/assets/user-account_settings.gif" alt="Account settings screens"><figcaption><p>Account settings screens</p></figcaption></figure>