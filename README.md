# pre-commit pyment

Mirror of pyment package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For pyment: see https://github.com/dadadel/pyment


### Using pyment with pre-commit

Add this to your `.pre-commit-config.yaml`:

    -   repo: https://github.com/hesstobi/pre-commit-pyment
        rev: ''  # Use the sha / tag you want to point at
        hooks:
        - id: pyment
          exclude: ^tests/
          args: ["-w", "-o", "numpydoc"]
