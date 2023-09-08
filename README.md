# maven-repository

[![GitHub license](https://img.shields.io/github/license/HighCapable/maven-repository-template?color=blue)](https://github.com/HighCapable/maven-repository-template/blob/main/LICENSE)

This is a simple Maven repository by using GitHub to manage dependencies.

这是一个使用 GitHub 管理依赖的简单 Maven 存储库。

## Usage

The directory `repository` is the repository, which contains two parts: `releases` (release version) and `snapshots` (snapshots), where all Maven project artifacts are stored.

Reference this repository using the link below.

> Releases

```
https://raw.githubusercontent.com/fankes/maven-repository/main/repository/releases
```

> SnapShots

```
https://raw.githubusercontent.com/fankes/maven-repository/main/repository/snapshots
```

### Usage in Gradle Projects

You can use this repository in any Gradle project.

#### Configure Repository

```kotlin
repositories {
    maven {
        name = "fankes-maven-releases"
        setUrl("https://raw.githubusercontent.com/fankes/maven-repository/main/repository/releases")
    }
    maven {
        name = "fankes-maven-snapshots"
        setUrl("https://raw.githubusercontent.com/fankes/maven-repository/main/repository/snapshots")
    }
}
```

You can also use [SweetDependency](https://github/HighCapable/SweetDependency) to uniformly manage and set up repositories.

```yaml
repositories:
  fankes-maven-releases:
    url: https://raw.githubusercontent.com/fankes/maven-repository/main/repository/releases
  fankes-maven-snapshots:
    url: https://raw.githubusercontent.com/fankes/maven-repository/main/repository/snapshots
```

## 使用方法

目录 `repository` 即为存储库，其中包含了 `releases` (发行版) 和 `snapshots` (快照) 两部分，这里存放了所有 Maven 项目的工件。

使用以下链接引用此存储库。

> Releases

```
https://raw.githubusercontent.com/fankes/maven-repository/main/repository/releases
```

> SnapShots

```
https://raw.githubusercontent.com/fankes/maven-repository/main/repository/snapshots
```

针对中国大陆地区无法访问 `raw.githubusercontent.com` 可以使用加速服务，例如 [GitMirror](https://gitmirror.com/)。

### 在 Gradle 项目中使用

你可以在任意 Gradle 项目中使用此存储库。

#### 配置存储库

```kotlin
repositories {
    maven {
        name = "fankes-maven-releases"
        setUrl("https://raw.githubusercontent.com/fankes/maven-repository/main/repository/releases")
    }
    maven {
        name = "fankes-maven-snapshots"
        setUrl("https://raw.githubusercontent.com/fankes/maven-repository/main/repository/snapshots")
    }
}
```

你还可以使用 [SweetDependency](https://github/HighCapable/SweetDependency) 统一管理并设置存储库。

```yaml
repositories:
  fankes-maven-releases:
    url: https://raw.githubusercontent.com/fankes/maven-repository/main/repository/releases
  fankes-maven-snapshots:
    url: https://raw.githubusercontent.com/fankes/maven-repository/main/repository/snapshots
```

## License

- [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0)

```
Apache License Version 2.0

Copyright (C) 2019-2023 HighCapable

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    https://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

Copyright © 2019-2023 HighCapable
