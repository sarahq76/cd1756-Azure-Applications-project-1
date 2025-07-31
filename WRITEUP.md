# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

I selected Azure App Service for deploying the CMS application because it simplifies the deployment process and removes the need for manual infrastructure management. It’s especially suitable for lightweight Flask applications like this one.

The integration with GitHub Actions made continuous deployment fast and straightforward, without the need to manually configure the server. App Service also provides native support for Python, environment variables, and built-in monitoring, which helped me stay focused on development instead of dealing with operational overhead.

Additionally, App Service is a cost-effective solution for projects that don’t require deep customization of the underlying operating system.

---

### When I Might Switch to a VM

There are certain scenarios where I would consider using a *Virtual Machine (VM)* instead:

If the app needed *custom libraries or services* at the OS level that App Service doesn’t support.
If I was working on a project with resource-heavy tasks, like real-time video processing or machine learning jobs.
If the app architecture became more complex and required tight control over multiple services or runtime environments* on the same host.

For now, however, Azure App Service offers a more practical and manageable solution given the app's current size and goals.


### Assess app changes that would change your decision.

If the app needed to integrate with a private network (via custom routing, VPNs, or hybrid cloud setups) or implement strict security controls that require admin-level access to firewalls and OS policies, a VM would be necessary to meet those needs.
