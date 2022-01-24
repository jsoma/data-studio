# Scribble

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

https://facelessuser.github.io/pymdown-extensions/extensions/arithmatex/

https://squidfunk.github.io/mkdocs-material/reference/admonitions/

=== ":octicons-arrow-right-16: inline end"

    !!! info inline end

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

    ``` markdown
    !!! info inline end
  
        Lorem ipsum dolor sit amet, consectetur
        adipiscing elit. Nulla et euismod nulla.
        Curabitur feugiat, tortor non consequat
        finibus, justo purus auctor massa, nec
        semper lorem quam in massa.
    ```

    Use `inline end` to align to the right (left for rtl languages).

=== ":octicons-arrow-left-16: inline"

    !!! info inline

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

    ``` markdown
    !!! info inline

        Lorem ipsum dolor sit amet, consectetur
        adipiscing elit. Nulla et euismod nulla.
        Curabitur feugiat, tortor non consequat
        finibus, justo purus auctor massa, nec
        semper lorem quam in massa.
    ```

    Use `inline` to align to the left (right for rtl languages).

!!! example "Injecting Classes"

    === "Unix, Powershell"

        ```
        docker run --rm -it -v ${PWD}:/docs squidfunk/mkdocs-material new .
        ```

    === "Windows"

        ```
        docker run --rm -it -v "%cd%":/docs squidfunk/mkdocs-material new .
        ```

!!! tip "Injecting Classes"

    ++ctrl+alt+delete++

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.


https://squidfunk.github.io/mkdocs-material/customization/?h=customiz#theme-development