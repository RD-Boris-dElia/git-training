# Tagging

Tagging is meant to capture a specific point in the git history that's marked for releasing.

There are two types of tags : lightweight and annotated.

It is important to semantic versioning standards when naming tags (like v1.0.0 or 1.0.0-alpha)

Check https://semver.org/ for details.

#### Annotated 

Stores metadata and allows for a description to be included with the tag.
It's usually best practice to use annotated tags over lightweight to have that additional info.

##### lightweight 

Only create the tag with its name.

## Let's tag !

- Create a tag v1.0.0 on your local
- Push the tag to your remote
- Add a feature3 file to your repo and push it
- Create a release with the tag v1.0.0

You'll see that the release won't contain your latest commit.
That's because a tag is like a snapshot of your repository at a given point.



