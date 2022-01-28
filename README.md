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
        root-url: <your root url>       # default: /
        modules: <your modules>         # required
        dir: <your checkout directory>  # default: .
```

