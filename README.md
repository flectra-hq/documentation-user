# Flectra documentation

## Build the documentation locally

### Requirements

- [Git](https://www.flectra.com/documentation/2.0/contributing/documentation/introduction_guide.html#install-git)
- [Python 3.6, 3.7, or 3.8](https://www.flectra.com/documentation/2.0/contributing/documentation/introduction_guide.html#python)
- Python dependencies listed in the file [`requirements.txt`](https://github.com/flectra/documentation/tree/2.0/requirements.txt).
- [Make](https://www.flectra.com/documentation/2.0/contributing/documentation/introduction_guide.html#make)
- A local copy of the [flectra/flectra repository in2.0](https://github.com/flectra/flectra/tree/2.0) (Optional)

### Instructions

1. In a terminal, navigate to the root directory and compile the documentation to HTML with the
   following command:

   ```sh
   make
   ```

   Additional commands are available with `make help`.

2. Open the file `documentation/_build/html/index.html` in your web browser to display the render.

3. See [this guide](https://www.flectra.com/documentation/2.0/contributing/documentation/introduction_guide.html#preview-your-changes)
   for more detailed instructions.

Optional: to fully build the developer documentation with inline docstrings for documented Python
functions, place your local copy of the `flectra/flectra` repository in the root directory. Alternatively,
create a symbolic link with `flectra` as link name. If the Flectra sources are not found, a warning will
be shown.

## Contribute to the documentation

For contributions to the content of the documentation, please refer to the
[Introduction Guide](https://www.flectra.com/documentation/2.0/contributing/documentation/introduction_guide.html).

To **report a content issue**, **request new content** or **ask a question**, use the
[repository's issue tracker](https://github.com/flectra/documentation-user/issues) as usual.

If you have a pull request that is ready for review, request one from the
[flectra/doc-review](https://github.com/orgs/flectra/teams/doc-review) team.


## Learn More

To learn more about Flectra, in addition to the documentation, have a look at
[the official eLearning](https://flectra.com/slides) and
[Scale-up, The Business Game](https://www.flectra.com/page/scale-up-business-game).