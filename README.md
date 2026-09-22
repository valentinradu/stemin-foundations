# Stemin Foundations

This is a content repository for [Stemin](https://git.kinoto.io/rad_val/stemin). It holds two
domains: mathematics (`math/`) and physics (`phy/`). The physics domain covers electricity and
magnetism, from charge to the electromagnetic wave.

## Use it

Add the address of this repository in the app, on the welcome page or with the `+`. The app
fetches the files, compiles them on your device, and keeps them there.

The host must be public, and it must send CORS headers. GitHub, GitLab and Codeberg do this.
A Forgejo or Gitea of your own needs `[cors] ENABLED = true` in its `app.ini`.

## Write it

The format is in `CONTENT-MODEL.md` in the Stemin repository. Check the repository before you
push:

```
stemin check .
```

The two domains stay in one repository on purpose. A reference from one domain to another works
only inside one repository, and physics will need mathematics.

This file is not content. The app reads only `index.md` and the directories that `order` names.
