# Let's Start To Cloud
Identity Access Management (IAM)

## Create User IAM
### Access type:
- Programmatic access: Enables an access key Id and secret access key for the AWS API, CLI, SDK, and other development tools
- AWS Management console access (aws dashboard)

### Permissions:
- Add user to a group
- Copy permissions from existing user
- Attach existing policies directly

Note: a group has multiples policies

## Exam Tips:
    - Identity Access Management (IAM) its global
    - Access to aws platform
        - Via the console (web dashboard)
        - Programatically (using the command line)
        - Using the software Developers kit (SDK)
    - Root account is the email address that created the account and has full administrator access
        - Not share this account
        - Always secure this account with M2FA
    - The users in a group will inherit all permissions that the group has
    - To set permissions to a group need to apply a policy to that group