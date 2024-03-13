## Motherduck and Malloy

[**Motherduck**](https://motherduck.com) is cloud based scale out relational SQL database.  

[**vscode.dev**](https://vscode.dev) is a web based version of VSCode that runs entirely in your browser. VSCode.dev can direcly work with github repositories from your web browser.  You can create make branches, edit files and push back to the repositories without need a local machine.

[**Malloy**](https://malloydata.dev) is a semantic data modeling and query language that among other things runs as an extension in VSCode.

Together these three components make a great way to explore and access data.

This repository is an example of using these three components together.  The example uses several datasets stored and shared in Motherduck.  Loading the datamodels from this repository, into Malloy in vscode will allow you to build and run data analysis against the data in Motherduck using only your browser.   You can modifiy these examples and/or follow this pattern with your own data.


To run these examples use

1. Goto https://app.motherduck.com and create an account
1. Goto https://insiders.vscode.dev/github/malloydata/motherduck-examples?vscode-coi=
1. Install the Malloy VSCode Extension (it should prompt you)
1. Goto Motherduck and click settings then 'Copy Token'
1. Open a Malloy file in the files pane for example [imdb.malloy](imdb/imdb.malloy).
1. Click on the 'M' in the right panel andd open Open Connections and make a new connection
    type: 'DuckDb' 
    name: 'md', 
    add your mother duck token
1. Run the Open [the attach data notebook](attach_data.malloynb)
1. Click 'Run All' to attach the example data to your motherduck database.

## Run any of the examples.

### FAA
* [Carrier Analysis](faa/carrier_analysis.malloynb)

### IMDB

* [IMDB overview](imdb/imdb.malloynb)
* [Genre Analysis](imdb/genre_analysis.malloynb)
* [Genre Matrix (genre co-occurance)](imdb/genre_matrix.malloynb)

### Ecommerce
* [Brand Synergy](ecommerce/brand_synergy.malloy)
