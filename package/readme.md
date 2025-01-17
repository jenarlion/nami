# How to add `exmaple` package

### Step 1

Create `exmaple.tengo`, write script to save commands into `$HOME/.nami/cache/`

### Step 2

Test `exmaple.tengo`, `nami install ./exmaple.tengo`

### Step 3

Fork nami project, put `exmaple.tengo` to package directory, create PR, then you can `nami install example`

OR

Put `exmaple.tengo` to your own http server, then you can `nami install https://yourserver.com/exmaple.tengo`

# Module - "nami"

```
nami := import("nami")
```

### Constants

-   `os`
-   `arch`
-   `home_dir`
-   `bin_dir`
-   `cache_dir`
-   `copied_dir`
-   `tmp_dir`

### Functions

-   `append_file(file string, text string) => error`: append data to file.
-   `write_file(file string, text string) => error`: write data to file.
-   `sh(name string, args...) => error`: run command
-   `sh1(name string, args...) => bytes/error`: run command and return stdout, 1
