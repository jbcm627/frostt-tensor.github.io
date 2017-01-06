# FROSTT
The **F**ormidable **R**epository of **O**pen **S**parse **T**ensors and
**T**ools.


## Project structure
The FROSTT website is written with [Jekyll](http://jekyllrb.com/) and has the
following project structure:
```
frostt.io/
  -  _layouts : Page layouts, including the dataset page layout.
  -  _pages   : A catch-all for pages.
  -  _posts   : News items.
  -  tensors  : Pages concerning the collection, that aren't actually tensors.
  -  _tensors : Markdown tensor pages.
  - scripts   : Scripts for generating tensor pages.
```


## Building
You can build and serve FROSTT for local development:
```
$ bundle install
$ jekyll serve --watch --detach
$ jekyll build --watch
```

Then just point your browser to [localhost:4000](localhost:4000). You can edit
any files and simply refresh the page. However, if you edit `_config.yml`, you
need to kill and restart the `jekyll build` command.


## Contributing
FROSTT thrives on community contributions. Pull requests and issues are
encouraged. To make a contribution, just fork this repository, create a branch
(with a descriptive name, please!), and issue a pull request through Github.

### Submitting a tensor

1. To submit a new tensor, copy the provided template `tensor-template.md`
to the `_tensors/` directory. The name of the file will form the URL of the
tensor page. Suppose your new tensor is named Big-Tensor:
  ```
  $ cp tensor-template.md _tensors/big-tensor.md
  ```

2. Fill in as much information as possible about your new tensor.

3. Build your tensor page. If all went well, your tensor should now exist.
Reload your local [FROSTT](http://localhost:4000/tensors/) page and Big-Tensor
should now be available.

4. Once the tensor page is ready, submit a pull request and include a public
link to the data in `files.txt`. We will copy the data to our hosting location,
update the links in `files.txt`, merge the pull request, and go live!


