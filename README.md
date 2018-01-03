# Bedrock documentation

Documentation and examples for the Bedrock framework.


## Setup

Take the following steps to set up and run the documentation site locally.


### Clone docs site

Clone the docs site to your local machine:

```
git clone git@github.com:ponysmith/bedrock-docs.git
```


### Jekyll

The Bedrock documentation site is built using [Jekyll](https://jekyllrb.com/). To run the documentation site locally, you will need to install Jekyll and Ruby. Follow the installation guidelines on the Jekyll site. For the best results, run the site with Ruby 2.3.


### Clone Bedrock site

The documentation site displays samples of Bedrock components, so it requires Bedrock itself to function properly. Install and setup Bedrock as follows:

Clone the Bedrock repository to your machine. To make installation as simple as possible, clone Bedrock into the same directory that the documentation site exists in.

```
git clone git@github.com:ponysmith/bedrock.git
```

Your setup should now look like this:

```
/ PARENT_DIRECTORY
  - bedrock
  - bedrock-docs
```


### Link Bedrock into the docs site

Create a symbolic link from the Bedrock code to within the `_sass` folder.

```
cd bedrock-docs/_sass
ln -s <path_to_bedrock_repo> bedrock
```


## Running the site

Once you have done all the setup, you can launch the site within

```
jekyll serve
```

## Making changes

Changes made to the documentation site itself should be reflected immediately if the server is running. If you make changes to files in the **bedrock** repo, you may need to stop and restart the Jekyll server.