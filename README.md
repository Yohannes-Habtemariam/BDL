# Generating a new SSH key and adding it to the ssh-agent 

After you've checked for existing SSH keys, you can generate a new SSH key to use for authentication, then add it to the ssh-agent. However, you need to know first your operating system. 

## Linus
The procedures are as follows: 
1. Open Terminal.
2. Paste the text below, substituting in your GitHub email address.

    $ ssh-keygen -t ed25519 -C "your_email@example.com"
3. When you're prompted to "Enter a file in which to save the key,"   press Enter. This accepts the default file location.
4. At the prompt, type a secure passphrase. For more information,   see "Working with SSH key passphrases."

Adding your SSH key to the ssh-agent
1. Start the ssh-agent in the background.
2. Add your SSH private key to the ssh-agent. If you created your key with a different name, or if you are adding an existing key that has a different name, replace id_ed25519 in the command with the name of your private key file.

    $ ssh-add ~/.ssh/id_ed25519

3. dd the SSH key to your account on GitHub. For more information, see "Adding a new SSH key to your GitHub account."
   

For further more detail information, you can read from [clicking here](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)