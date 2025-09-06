# cv-backbone-notes
My notes and comments on popular computer vision backbone source codes


## To maintain annotations with github submodule

1. Add a submodule (which is a "child" github repo) to the parent:

    ```
    git submodule add https://github.com/google-research/vision_transformer.git 20_ViT
    ```
    Note that don't have to fork it.

1. After making changes in the submodules


1. To completely delete a submodule:

    ```
    git submodule deinit -f path/to/submodule
    git rm --cached path/to/submodule
    rm -rf <path_to_submodule>
    git config -f .gitmodules --remove-section submodule.<submodule_name>

    rm -rf .git/modules/path/to/submodule
    git rm -f path/to/submodule
    ```

1. To check submodule status:
    ```
    git submodule status
    ```

