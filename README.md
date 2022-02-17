# actions-doc-gen4
GitHub Action for doc-gen4

## Usage

```yaml
    steps:
    - name: Checkout
      uses: actions/checkout@v2
    - name: Generate Documentation
      uses: xubaiw/actions-doc-gen4@master
      with:
        root-url: <your repo>                         # e.g. /Socket.lean/
        modules: <your modules>                       # e.g. Socket
        dir: <your checkout directory>                # default: .
        doc-gen4-repo: <alternative docgen repo>      # default: https://github.com/leanprover/doc-gen4.git
        doc-gen4-repo: <alternative docgen checkout>  # default: main


    - name: Deploy
        uses: JamesIves/github-pages-deploy-action@v4.2.2
        with:
          branch: gh-pages 
          folder: build/doc
```

