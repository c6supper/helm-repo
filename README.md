# Helm Charts Repo

This is my private helm charts repository.

### How It Works

I set up GitHub Pages to point to the root folder. From there, I can
create and publish like this:

```console
$ helm create mychart
$ helm package mychart
$ helm repo index ./ --url https://c6supper.github.com/helm-repo
$ git add -i
$ git commit -av
$ git push origin master
```

From there, I can do a `helm repo add helm-repo
https://c6supper.github.com/helm-repo`
