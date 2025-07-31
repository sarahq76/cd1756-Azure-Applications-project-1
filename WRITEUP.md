# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

Because Azure App Service streamlines the deployment process and eliminates the need for manual infrastructure management, I decided to use it to deploy the CMS application. For lightweight Flask applications like this one, it works particularly well.

Continuous deployment was made quick and simple by the integration with GitHub Actions, which eliminated the need for manual server configuration. Additionally, App Service has built-in monitoring, environment variables, and native support for Python, all of which allowed me to concentrate on development rather than operational overhead.

Furthermore, App Service is an affordable option for projects that don't call for extensive operating system customization.

---

### When I Might Switch to a VM

There are certain scenarios where I would consider using a VM instead:

If the app needed *custom libraries or services* at the OS level that App Service doesn’t support.
If I was working on a project with resource-heavy tasks, like real-time video processing or machine learning jobs.
If the app architecture became more complex and required tight control over multiple services or runtime environments* on the same host.

For now, however, Azure App Service offers a more practical and manageable solution given the app's current size and goals.


### Assess app changes that would change your decision.

If the app needed to integrate with a private network (via custom routing, VPNs, or hybrid cloud setups) or implement strict security controls that require admin-level access to firewalls and OS policies, a VM would be necessary to meet those needs.
