# getpopper.io website

This is the repository for the getpopper.io webpage. It uses the 
[Docsy](https://github.com/google/docsy), which is a 
[Hugo](https://gohugo.io) theme for technical documentation sites, 
providing easy site navigation, structure, and more. You can find 
detailed theme instructions in the Docsy user guide at 
<https://docsy.dev/docs>

This website is hosted at <https://getpopper.github.io/website>.

## Running the website locally

Once you've cloned the site repo, from the repo root folder, run:

```bash
docker run --rm -it \
  --volume $(PWD):/src \
  --volume $(PWD)/public:/target \
  --publish 1313:1313 \
  klakegg/hugo:0.67.0-ext server
```

To deploy the website:

```bash
./deploy.sh
```
