# aws-amp-docs
### Testing AWS Amplify to host static site using mkdocs

Generating the docs
----------

NOTE: best practices is to do this from a virtual environment.  This requires Python 3.

Install requirements from the repository root directory:

    pip3 install -r requirements.txt

Change directories into the docs folder:

    cd docs

Use [mkdocs](http://www.mkdocs.org/) structure to update the documentation. Test locally with:

    mkdocs serve

You can view the documents at (http://localhost:8000).  If you are developing documentation,
the server will refresh the site each time a file - content or configuration - is updated.

Once the docs look good, publish to AWS Amplify by submitting a pull request from the development branch to the `docs` branch.
Once the pull request is merged onto the target `docs`, the automated build and deploy scripts will build and deploy the documentation using AWS Amplify.

** Note **: Never edit the generated site by hand.
