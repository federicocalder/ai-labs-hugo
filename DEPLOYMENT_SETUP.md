# GitHub Secrets Setup Instructions

You need to add these secrets to your GitHub repository:

1. Go to: https://github.com/federicocalder/ai-labs-hugo/settings/secrets/actions

2. Add these secrets:

   **SERVER_HOST**
   Value: 5.78.131.81

   **SERVER_USER**  
   Value: root

   **SERVER_SSH_KEY**
   Value: Your private SSH key content
   (The same key you use to SSH to the server)

## How to get your SSH key:

Run this command on your Mac:
```bash
cat ~/.ssh/id_rsa
```

Copy the entire output (including -----BEGIN and -----END lines) 
and paste it as the SERVER_SSH_KEY secret value.

## After adding secrets:

The GitHub Actions workflow will automatically deploy on every push to main branch.

## Manual trigger:

You can also trigger deployment manually from:
https://github.com/federicocalder/ai-labs-hugo/actions
