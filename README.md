# rebasing-hook

Rebasing helper: be notified when your rebase results in code changes

# What is this?

A tool to show you the diff caused by your rebases, with a friendly way of
discarding your changes if you so wish:

![Confirmation dialogue after rebase](https://images.thoughtbot.com/blog-vellum-image-uploads/Z7y7SFJTR0OXp9pwlQEr_Screenshot%202020-04-24%20at%2012.19.40.png)

# Installation

## Add the hooks to a project

Simply copy all files under this repository's `/hook` folder to your `.git/hooks`
in your project.

## Add to your default Git initialisation

You can copy the hooks to your Git template folder and they will be automatically
setup every time you run `git init`. If you don't have a template folder set, the
following commands will create a template for you, including this rebasing hook:

```bash
mkdir ~/.git-template
cp -r hooks/ ~/.git-template/hooks
git config --global init.templatedir '~/.git-template'
```


Happy rebasing :)
