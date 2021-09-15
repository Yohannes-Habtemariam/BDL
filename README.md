# Generating a new SSH key and adding it to the ssh-agent
After you've checked for existing SSH keys, you can generate a new SSH key to use for authentication, then add it to the ssh-agent. You need to consider the operating system of your computer. 

## Linus
1. Open Terminal.

2. Paste the text below, substituting in your GitHub email address.

   $ ssh-keygen -t ed25519 -C "your_email@example.com"
