## Container Images Assignment

**Note:** This assumes you have your SSH key uploaded to your GH account.
If you do not, replace `git@github.com:name/repo.git` to
`https://github.com/name/repo.git`

### Step 0

```bash
cd spark-seprep
git fetch --all
git rebase upstream/main
git push origin main # this is to update your remote fork, it's a good habit
git checkout -b pacman

# or if you removed or need to re-clone the repo,
git clone git@github.com:yourghname/spark-seprep.git
cd spark-seprep
git remote add upstream git@github.com:DS219/spark-seprep.git
git rebase upstream/main
# if there are problems, try `git reset --hard upstream/main`
git push origin main # this is to update your remote fork, it's a good habit
git checkout -b pacman
```

### Option 1

Sign up for a free account on [DockerHub](https://hub.docker.com/).
Complete the [pacman tutorial](https://github.com/umohnani8/fun-work/blob/main/tutorials/pacman-ctr.md).
When you build your image, tag it as `docker.io/yourdockerusername/pacman:latest`
With your new DockerHub account, you can push your container image.
Run this:

```bash
podman login -u dockerusername -p yourpassword docker.io
podman push docker.io/yourdockerusername/pacman:latest
```

Now, share the name of your container image to your named file that lives at
`./assignments/pacman/yourbu-name.md`

Add anything else in that file, if you had trouble running or pushing the image,
or if you have any other questions, feel free to add it to that file.

**Bonus**: Use some [markdown styling](https://www.markdownguide.org/cheat-sheet/)

Finish the assigment by following [PR creation](#create-a-pr) section.

### Option 2

Complete the [pacman tutorial](https://github.com/umohnani8/fun-work/blob/main/tutorials/pacman-ctr.md).

Run the following:

```
podman logs pacman
```

Now, copy/paste the output of the above command from your terminal to a file at
`./assignments/pacman/yourbu-name.md`

Add anything else in that file, if you had trouble running or pushing the image,
or if you have any other questions, feel free to add it to that file.

**Bonus**: Use some [markdown styling](https://www.markdownguide.org/cheat-sheet/)

Finish the assigment by following [PR creation](#create-a-pr) section.

### Create a PR

Now create a pull request to the github.com/DS219/spark-seprep repository.

Run the following:

```bash
git add .
git commit -m "yourname: container images assignment"
git push origin pacman
```

Now go to the GitHub UI and create a PR, comparing your pacman branch against
DS219/spark-seprep main branch. 

