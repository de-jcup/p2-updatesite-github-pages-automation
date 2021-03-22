# p2-updatesite-github-pages-automation
A p2 eclipse update site automation approach by simple script + GitHub actions.

## How to use
Let's assume your projects name is `alpha`.

### Initial/Prepare
For first time you will need to do following steps to prepare:

1. copy `deploy.sh` into repository root of project `alpha` - change GITHUB user name variable
2. ensure inside project `alpha` the eclipse project folder with the update-site ends with `updatesite`
3. create a new repository called `update-site-alpha`
4. copy `snippets/update-site_index.md` as `index.md` into `update-site-alpha/update-site/` (landing page)

### Update mechanism
1. build your eclipse plugin and features
2. call `./deploy.sh` (if there are missing environment variables, the script will tell you)

