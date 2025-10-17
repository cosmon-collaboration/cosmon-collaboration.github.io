Home page for CoSMoN using Hugo.

In order to test locally, make sure to have the `extended` version of [Hugo installed](https://gohugo.io/installation/).  Then,
```
git clone --recursive git@github.com:cosmon-collaboration/cosmon-collaboration.github.io.git
cd cosmon-collaboration.github.io
git submodule update --remote --recursive
hugo serve
```
This should launch a webpage locally that you can view at the site:
```
http://localhost:1313/
```
or whichever address the prompt from the terminal tells you.  If this does not work, then stop serving the site, and do
```
bash themes/hugo-texademic/scripts/add_npm_modules.sh
```
and then try serving the site again.  If this still does not work, contact André.

After you have a working site, you can add new content by making a new branch
```
git checkout -b <branch_name>
```
add content, make sure it works locally, add the new files
```
git add <files you added/modified>
git commit -m "some useful message"
git push
```
and then issue a pull request to the `main` branch.
