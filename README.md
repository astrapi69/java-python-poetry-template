# Java-Python Poetry Template

<div style="text-align: center">

[![Build Status](https://github.com/astrapi69/java-python-poetry-template/actions/workflows/gradle.yml/badge.svg)](https://github.com/astrapi69/java-python-poetry-template/actions/workflows/gradle.yml)
[![Coverage Status](https://codecov.io/gh/astrapi69/java-python-poetry-template/branch/develop/graph/badge.svg)](https://codecov.io/gh/astrapi69/java-python-poetry-template)
[![Open Issues](https://img.shields.io/github/issues/astrapi69/java-python-poetry-template.svg?style=flat)](https://github.com/astrapi69/java-python-poetry-template/issues)
[![Maven Central](https://img.shields.io/maven-central/v/io.github.astrapi69/java-python-poetry-template?style=plastic)](https://search.maven.org/artifact/io.github.astrapi69/java-python-poetry-template)
[![Javadocs](http://www.javadoc.io/badge/io.github.astrapi69/java-python-poetry-template.svg)](http://www.javadoc.io/doc/io.github.astrapi69/java-python-poetry-template)
[![MIT License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](http://opensource.org/licenses/MIT)
[![Donate](https://img.shields.io/badge/donate-❤-ff2244.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GVBTWLRAZ7HB8)
[![Hits Of Code](https://hitsofcode.com/github/astrapi69/java-python-poetry-template?branch=develop)](https://hitsofcode.com/github/astrapi69/java-python-poetry-template/view?branch=develop)

</div>

## Overview

A template repository for Java and Python projects using Gradle and Poetry. The Java project is configured with Gradle for dependency management and build automation, while the Python project utilizes Poetry for package management and environment configuration. This repository provides a structured starting point for new projects. A small documentation on how to use this template project can be found in the [wiki](https://github.com/astrapi69/java-python-poetry-template/wiki).

> Please support this project by starring it on GitHub ⭐
> If you find this useful, consider sharing it with others!
> [![Donate](https://img.shields.io/badge/donate-❤-ff2244.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GVBTWLRAZ7HB8)

---

## Usage

### Java (Gradle)
See the **Gradle** section below for details on how to import dependencies.

### Python (Poetry)

This template includes **Poetry** for managing Python dependencies.

#### **1. Install Poetry**
Ensure Poetry is installed on your system:

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

Verify installation:

```bash
poetry --version
```

#### **2. Install Dependencies**
Run the following command to install dependencies:

```bash
poetry install
```

#### **3. Run the Python Application**
To execute the Python project, use:

```bash
poetry run python main.py
```

#### **4. Add New Dependencies**
To add a new package:

```bash
poetry add <package-name>
```

For development dependencies:

```bash
poetry add --dev <package-name>
```

#### **5. Virtual Environment Configuration (Optional)**
To keep the virtual environment inside the project directory:

```bash
poetry config virtualenvs.in-project true
```

#### **6. Updating Dependencies**
To update all dependencies to their latest allowed versions:

```bash
poetry update
```

---

## Import dependencies to your project

<details>
  <summary>Gradle (click to expand)</summary>

### Gradle Dependency

Replace `${latestVersion}` with the latest version:
[![Maven Central](https://img.shields.io/maven-central/v/io.github.astrapi69/java-python-poetry-template?style=plastic)](https://search.maven.org/artifact/io.github.astrapi69/java-python-poetry-template)

#### **Define version in `gradle.properties`**
```properties
javaPythonPoetryTemplateVersion=${latestVersion}
```

or in `build.gradle`
```groovy
javaPythonPoetryTemplateVersion = "${latestVersion}"
```

#### **Add dependency in `build.gradle`**
```groovy
dependencies {
    implementation("io.github.astrapi69:java-python-poetry-template:$javaPythonPoetryTemplateVersion")
}
```

#### **With `libs.versions.toml`**
```toml
[versions]
java-python-poetry-template-version= "${latestVersion}"

[libraries]
java-python-poetry-template = { module = "io.github.astrapi69:java-python-poetry-template", version.ref = "java-python-poetry-template-version" }
```

Then use:

```groovy
dependencies {
    implementation libs.java.python.poetry.template
}
```

</details>

<details>
  <summary>Maven (click to expand)</summary>

### Maven Dependency

Check out the latest snapshots and releases on [Sonatype Repository](https://oss.sonatype.org/index.html#nexus-search;gav~io.github.astrapi69~java-python-poetry-template~~~).

#### **Add dependency in `pom.xml`**
```xml
<properties>
    <java-python-poetry-template.version>${latestVersion}</java-python-poetry-template.version>
</properties>

<dependencies>
    <dependency>
        <groupId>io.github.astrapi69</groupId>
        <artifactId>java-python-poetry-template</artifactId>
        <version>${java-python-poetry-template.version}</version>
    </dependency>
</dependencies>
```

</details>

---

## Donations

If you like this project, consider supporting it via:

- **[PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=MJ7V43GU2H386)**
- Bitcoin: `bc1ql2y99q7e8psndhcc3gferk03esw3qqf677rhjy`
- Ethereum: `0xc057D159D3C8f3311E73568b334FF6fE82EB2b7D`
- Monero: `49bqeRQ7Bf49oJFVC72pqpe5hFbb62pfXDYPdLsadGGF81KZW2ZfrPZ8PbAVu5X2v1TYAspeczMya3cYQysNS4usRRPQHVw`

---

## Semantic Versioning

This repository follows [Semantic Versioning](https://semver.org/):

```
<major>.<minor>.<patch>
```

---

## How to Support

- ⭐ Star this repository
- 📥 Submit feature requests or bug reports
- 💡 Contribute by solving issues or submitting pull requests

---

## Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests.

---

## Contact

For issues and feature requests, visit the [Issues page](https://github.com/astrapi69/java-python-poetry-template/issues).

---
