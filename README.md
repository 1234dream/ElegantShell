# ElegantShell

ElegantShell 是一个简洁而强大的命令行界面，旨在提供一种易于使用和扩展的shell体验。它包括基本命令处理功能和一个可扩展的框架，允许贡献者添加更多功能。

## 获取项目

要开始使用和开发 ElegantShell，首先将项目仓库克隆到您的本地环境：

```bash
git clone [仓库URL]
```

## 构建项目

在项目的根目录下，运行以下命令来编译 ElegantShell：

```bash
make all
```

这将编译项目并生成 `ElegantShell` 可执行文件。

## 运行 ElegantShell

编译完成后，在项目根目录下运行：

```bash
./ElegantShell
```

这将启动 ElegantShell。

## 已实现的功能

- **`hello` 命令**: 基本命令示例。
- **`tree` 命令**: 显示目录结构，具有颜色高亮和文件-目录计数的特性。
- **输入输出重定向**: 允许重定向命令的输入和输出。
- **`wc` 命令**: 统计指定文件或输入中的行数、单词数和字符数。
- **管道 (`|`)**: 允许将一个命令的输出作为另一个命令的输入。
- **后台运行 (`&`)**: 允许程序在后台运行。
- **`ls`**: 列出指定目录下的文件和文件夹。
- **`cd`**: 切换工作目录。
- **`clear`**: 清空屏幕。
- **`pwd`**: 显示当前工作目录路径。
- **`mkdir`**: 创建新目录。
- **`help`/`man`**: 显示命令帮助信息。
- **`ps`**: 显示进程信息。
- **`history`**: 显示命令历史记录。

## 待实现的功能

- **`mv`**: 移动或重命名文件和文件夹。
- **`rm`**: 删除文件或文件夹。
- **`cp`**: 复制文件或文件夹。

## 测试和开发

我们欢迎贡献者进行测试和开发。您可以在 `src` 目录下找到命令的实现模板。目前，`src` 目录包含一个 `hello` 命令作为示例。

### 添加新命令

1. 在 `src` 目录下创建您的命令实现文件，例如 `mycommand.c`。
2. 在相应的头文件（如 `mycommand.h`）中声明您的命令。
3. 在 `main.c` 或其他合适的地方注册您的新命令。

### 提交更改

1. 在本地进行充分测试后，提交您的更改到您的分支。
2. 创建一个 Pull Request，详细描述您的更改和改进。
3. 请求其他团队成员审查您的代码，并合并到主分支。

## License

本项目遵循 [LICENSE](./LICENSE) 下的条款。在使用、修改或分发本项目代码时，请确保遵守相应的许可协议。