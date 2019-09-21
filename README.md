# To deploy this:
```sh
# Set up theme
git submodule init
git submodule update

# Build
hugo

# Switch to public branch
git checkout master

# Copy files to deploy
cp -r public/* .
rm -rf public/ themes/

# Commit and publish
git commit --all -m "Deploy changes"
git push
```
