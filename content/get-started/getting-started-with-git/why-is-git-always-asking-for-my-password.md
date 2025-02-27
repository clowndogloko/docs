---
title: Why is Git always asking for my password?
intro: 'If Git prompts you for a username and password every time you try to interact with GitHub, you''re probably using the HTTPS clone URL for your repository.'
redirect_from:
  - /articles/why-is-git-always-asking-for-my-password
  - /github/using-git/why-is-git-always-asking-for-my-password
  - /github/getting-started-with-github/why-is-git-always-asking-for-my-password
  - /github/getting-started-with-github/getting-started-with-git/why-is-git-always-asking-for-my-password
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
shortTitle: Git passwords
---
Using an HTTPS remote URL has some advantages compared with using SSH. It's easier to set up than SSH, and usually works through strict firewalls and proxies. However, it also prompts you to enter your {% data variables.product.product_name %} credentials every time you pull or push a repository. 

{% data reusables.user-settings.password-authentication-deprecation %}

You can avoid being prompted for your password by configuring Git to [cache your credentials](/get-started/getting-started-with-git/caching-your-github-credentials-in-git) for you. Once you've configured credential caching, Git automatically uses your cached {% data variables.product.pat_generic %} when you pull or push a repository using HTTPS.

## Further reading

- "[About remote repositories](/get-started/getting-started-with-git/about-remote-repositories)."
- "[About authentication to {% data variables.product.prodname_dotcom %}](/authentication/keeping-your-account-and-data-secure/about-authentication-to-github)"
- "[Adding your SSH key to the ssh-agent](/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent)"
