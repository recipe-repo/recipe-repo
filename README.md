# Recipe-Repo

Recipe-Repo is a self-hosted recipe manager which aims to make it easy to store and share your recipes while maintaining full control over them.

### Why make Recipe-Repo?

Recipe-Repo is being made with the knowledge that every service dies someday. Many recipe managers force you to save recipes to remote servers which you can only access through an app or webpage. In order to use a different recipe manager you have a herculean task of re-entering every recipe by hand as there's no way to export. Or maybe the servers will just suddenly shut down taking all your recipes with them.

Recipe-Repo gives you control over all your data. Every recipe remains on your own computer stored in a MongoDB database so you will always be able to access them.

#### Please note:
Recipe-Repo's currently in the very early stages of development, things will get broken so do not rely on being able to migrate recipes between versions.

Recipe-Repo currently has no form of authentication on the frontend. Do not make Recipe-Repo publicly accessible.

---

### Features

In the current version you can:

- Create and view recipes
- Edit and delete recipes

### Roadmap

There's currently plans to allow:

- Making shopping lists (exporting lists to Trello/etc.)
- Automated recipe imports
- Searching for recipes by name/ingredients/etc.
- Share recipes by email/etc.

If there's any features you want to see, feel free to open an issue to discuss.

---

### Getting Started

It's very easy to get started with Recipe-Repo. Once you have set up Docker in swarm mode, simply download [docker-compose.yaml](docker-compose.yaml) and run the command

```sh
$ docker stack deploy RecipeRepo --compose-file=docker-compose.yaml
```

### Updating to a new version

You can move to the new version of Recipe-Repo by updating the image tags in `docker-compose.yaml` or just downloading the new version posted here and then rerunning the above command.
