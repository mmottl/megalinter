<!-- markdownlint-disable MD033 MD041 -->
<!-- Generated by .automation/build.py, please do not update manually -->

<div align="center">
  <a href="https://www.sqlfluff.com/" target="blank" title="Visit linter Web Site">
    <img src="https://raw.githubusercontent.com/sqlfluff/sqlfluff/master/images/sqlfluff-wide.png" alt="sqlfluff" height="150px" class="megalinter-banner">
  </a>
</div>

## sqlfluff documentation

- Version in Mega-Linter: **0.4.0**
- Visit [Official Web Site](https://www.sqlfluff.com/){target=_blank}
- See [How to configure sqlfluff rules](https://docs.sqlfluff.com/en/stable/configuration.html){target=_blank}
- See [Index of problems detected by sqlfluff](https://docs.sqlfluff.com/en/stable/rules.html){target=_blank}

[![sqlfluff - GitHub](https://gh-card.dev/repos/sqlfluff/sqlfluff.svg?fullname=)](https://github.com/sqlfluff/sqlfluff){target=_blank}

## Configuration in Mega-Linter

- Enable sqlfluff by adding `SQL_SQLFLUFF` in [ENABLE_LINTERS variable](https://nvuillam.github.io/mega-linter/configuration/#activation-and-deactivation)
- Disable sqlfluff by adding `SQL_SQLFLUFF` in [DISABLE_LINTERS variable](https://nvuillam.github.io/mega-linter/configuration/#activation-and-deactivation)

| Variable                                 | Description                                                                                                                                                                                  | Default value                                    |
|------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------|
| SQL_SQLFLUFF_ARGUMENTS                   | User custom arguments to add in linter CLI call<br/>Ex: `-s --foo "bar"`                                                                                                                     |                                                  |
| SQL_SQLFLUFF_FILTER_REGEX_INCLUDE        | Custom regex including filter<br/>Ex: `(src|lib)`                                                                                                                                            | Include every file                               |
| SQL_SQLFLUFF_FILTER_REGEX_EXCLUDE        | Custom regex excluding filter<br/>Ex: `(test|examples)`                                                                                                                                      | Exclude no file                                  |
| SQL_SQLFLUFF_FILE_EXTENSIONS             | Allowed file extensions. `"*"` matches any extension, `""` matches empty extension. Empty list excludes all files<br/>Ex: `[".py", ""]`                                                      | `[".sql"]`                                       |
| SQL_SQLFLUFF_FILE_NAMES_REGEX            | File name regex filters. Regular expression list for filtering files by their base names using regex full match. Empty list includes all files<br/>Ex: `["Dockerfile(-.+)?", "Jenkinsfile"]` | Include every file                               |
| SQL_SQLFLUFF_CONFIG_FILE                 | sqlfluff configuration file name</br>Use `LINTER_DEFAULT` to let the linter find it                                                                                                          | `setup.cfg`                                      |
| SQL_SQLFLUFF_RULES_PATH                  | Path where to find linter configuration file                                                                                                                                                 | Workspace folder, then Mega-Linter default rules |
| SQL_SQLFLUFF_DISABLE_ERRORS              | Run linter but consider errors as warnings                                                                                                                                                   | `false`                                          |
| SQL_SQLFLUFF_DISABLE_ERRORS_IF_LESS_THAN | Maximum number of errors allowed                                                                                                                                                             | `0`                                              |

## Mega-Linter Flavours

This linter is available in the following flavours

| <!-- -->                                                                                                                                                  | Flavor                                                                         | Description                                           | Embedded linters | Info                                                                                                                                                                                               |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------|-------------------------------------------------------|------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/images/mega-linter-square.png" alt="" height="32px" class="megalinter-icon"></a> | [all](https://nvuillam.github.io/mega-linter/supported-linters/)               | Default Mega-Linter Flavor                            | 84               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter)                             |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/dart.ico" alt="" height="32px" class="megalinter-icon"></a>                | [dart](https://nvuillam.github.io/mega-linter/flavors/dart/)                   | Optimized for DART based projects                     | 38               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-dart/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-dart)                   |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/documentation.ico" alt="" height="32px" class="megalinter-icon"></a>       | [documentation](https://nvuillam.github.io/mega-linter/flavors/documentation/) | Mega-Linter for documentation projects                | 37               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-documentation/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-documentation) |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/dotnet.ico" alt="" height="32px" class="megalinter-icon"></a>              | [dotnet](https://nvuillam.github.io/mega-linter/flavors/dotnet/)               | Optimized for C, C++, C# or VB based projects         | 43               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-dotnet/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-dotnet)               |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/go.ico" alt="" height="32px" class="megalinter-icon"></a>                  | [go](https://nvuillam.github.io/mega-linter/flavors/go/)                       | Optimized for GO based projects                       | 39               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-go/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-go)                       |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/java.ico" alt="" height="32px" class="megalinter-icon"></a>                | [java](https://nvuillam.github.io/mega-linter/flavors/java/)                   | Optimized for JAVA based projects                     | 38               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-java/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-java)                   |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/javascript.ico" alt="" height="32px" class="megalinter-icon"></a>          | [javascript](https://nvuillam.github.io/mega-linter/flavors/javascript/)       | Optimized for JAVASCRIPT or TYPESCRIPT based projects | 46               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-javascript/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-javascript)       |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/php.ico" alt="" height="32px" class="megalinter-icon"></a>                 | [php](https://nvuillam.github.io/mega-linter/flavors/php/)                     | Optimized for PHP based projects                      | 41               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-php/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-php)                     |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/python.ico" alt="" height="32px" class="megalinter-icon"></a>              | [python](https://nvuillam.github.io/mega-linter/flavors/python/)               | Optimized for PYTHON based projects                   | 44               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-python/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-python)               |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/ruby.ico" alt="" height="32px" class="megalinter-icon"></a>                | [ruby](https://nvuillam.github.io/mega-linter/flavors/ruby/)                   | Optimized for RUBY based projects                     | 38               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-ruby/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-ruby)                   |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/rust.ico" alt="" height="32px" class="megalinter-icon"></a>                | [rust](https://nvuillam.github.io/mega-linter/flavors/rust/)                   | Optimized for RUST based projects                     | 38               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-rust/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-rust)                   |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/salesforce.ico" alt="" height="32px" class="megalinter-icon"></a>          | [salesforce](https://nvuillam.github.io/mega-linter/flavors/salesforce/)       | Optimized for Salesforce based projects               | 38               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-salesforce/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-salesforce)       |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/scala.ico" alt="" height="32px" class="megalinter-icon"></a>               | [scala](https://nvuillam.github.io/mega-linter/flavors/scala/)                 | Optimized for SCALA based projects                    | 38               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-scala/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-scala)                 |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/swift.ico" alt="" height="32px" class="megalinter-icon"></a>               | [swift](https://nvuillam.github.io/mega-linter/flavors/swift/)                 | Optimized for SWIFT based projects                    | 38               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-swift/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-swift)                 |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/terraform.ico" alt="" height="32px" class="megalinter-icon"></a>           | [terraform](https://nvuillam.github.io/mega-linter/flavors/terraform/)         | Optimized for TERRAFORM based projects                | 40               | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-terraform/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-terraform)         |

## Behind the scenes

### How are identified applicable files

- File extensions: `.sql`

<!-- markdownlint-disable -->
<!-- /* cSpell:disable */ -->

### Example calls

```shell
sqlfluff myfile.sql
```


### Help content

```shell
Usage: sqlfluff [OPTIONS] COMMAND [ARGS]...

  Sqlfluff is a modular sql linter for humans.

Options:
  --version  Show the version and exit.
  --help     Show this message and exit.

Commands:
  dialects  Show the current dialects available.
  fix       Fix SQL files.
  lint      Lint SQL files via passing a list of files or using stdin.
  parse     Parse SQL files and just spit out the result.
  rules     Show the current rules in use.
  version   Show the version of sqlfluff.
```

### Installation on mega-linter Docker image

- PIP packages (Python):
  - [sqlfluff](https://pypi.org/project/sqlfluff)