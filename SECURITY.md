# Security policy

1. [Reporting security problems to PRTriage](#reporting)
2. [Security Point of Contact](#contact)
3. [Incident Response Process](#process)
4. [Vulnerability Management Plan](#vulnerability-management)

<a name="reporting"></a>
## Reporting security problems to PRTriage

**CREATE AN ISSUE** to report a security problems.

<a name="contact"></a>
## Security Point of Contact

The security point of contact is Sam Yamashita. Sam responds to security
incident reports as fast as possible, within one business day at the latest.

If Sam does not respond then please contact support@github.com
who can disable any access for the PRTriage app until the security incident is resolved.

<a name="process"></a>
## Incident Response

In case an incident is discovered or reported, I will follow the following
process to contain, respond and remediate:

### 1. Containment

The first step is to find out the root cause, nature and scope of the incident.

- Is still ongoing? If yes, first priority is to stop it.
- Is the incident outside of my influence? If yes, first priority is to contain it.
- Find out knows about the incident and who is affected.
- Find out what data was potentially exposed.

One way to immediately remove all access for the PRTriage app is to remove the
private key from the PRTriage App Settings page. The access can be recovered later
by generating a new private key and re-deploy the app.

### 2. Response

After the initial assessment and containment to my best abilities, I will
document all actions taken in a response plan.

I will create a comment in [the official "Updates" issue](https://github.com/wip/app/issues/89) to inform users about
the incident and what I actions I took to contain it.

### 3. Remediation

Once the incident is confirmed to be resolved, I will summarize the lessons
learned from the incident and create a list of actions I will take to prevent
it from happening again.

<a name="vulnerability-management"></a>
## Vulnerability Management Plans

### Keep permissions to a minimum

The PRTriage App uses the least amount of access to limit the impact of possible
security incidents, see [Information collection and use](PRIVACY.md#information-collection-and-use).

If someone would get access to the PRTriage app, the worst thing they could do is to
read out contents from pull requests, limited to repositories the PRTriage got
installed on.

### Secure accounts with access

The [PRTriage GitHub Organization](https://github.com/pr-triage) requires 2FA authorization
for all members.

### Critical Updates And Security Notices

We learn about critical software updates and security threats from these sources

1. GitHub Security Alerts
1. [Greenkeeper](https://greenkeeper.io/) Dependency Updates
1. GitHub: https://status.github.com/ & [@githubstatus](https://twitter.com/githubstatus)
1. Snyk (Vulnerabilities): https://snyk.statuspage.io/ & [@snyksec](https://twitter.com/snyksec)
1. Glitch (Hosting): https://status.glitch.com/ & [@glitch](https://twitter.com/glitch?lang=ens)
1. Travis (CI/CD): https://www.traviscistatus.com/ & [@traviscistatus](https://twitter.com/traviscistatus)
