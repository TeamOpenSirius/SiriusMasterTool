# SiriusMasterTool

《World Dai Star》官方 MasterData 下载与更新工具。

## 项目结构

```text
Cli/             命令行解析和帮助
Configuration/   下载与认证选项
MasterData/      MasterMemory 导出和发布模型
Networking/      官方 API、协议流和下载客户端
Persistence/     本地同步状态
Protocol/        工具专用 MessagePack DTO
data/            MasterData 表结构
Program.cs       程序入口与同步流程
```

## 编译

```powershell
dotnet build Sirius.MasterTool.sln -c Release
```

## 运行

```powershell
.\bin\Release\net10.0\Sirius.MasterTool.exe --sync --dir output
```

运行 `Sirius.MasterTool.exe --help` 查看认证及更新选项。
