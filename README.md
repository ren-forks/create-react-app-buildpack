Heroku React builtpack - Ren fork
=================================

See [mars/create-react-app-buildpack](https://github.com/mars/create-react-app-buildpack) for full instructions.

## Initial setup

In your git reposistory, add your Heroku project's git remote:

```sh
git remote add heroku https://git.heroku.com/project-name.git
```

If the React app is in a subdirectory of your git repository, see [subdir-heroku-buildpack](https://github.com/timanovsky/subdir-heroku-buildpack).

Next, set up this Heroku buildpack:

```sh
heroku buildpacks:clear
heroku buildpacks:set https://github.com/ren-forks/create-react-app-buildpack.git
```

Finally, push to the Heroku git remote (replacing `yourbranch` with the branch you are pushing from):

```sh
git push heroku yourbranch:master
```

## Deploying new changes

Same as the last step of the intial setup:

```sh
git push heroku yourbranch:master
```
