# SHENZHEN I/O 本地构建工程

工程目标为 .NET Framework 4.5.1、x86。将自备的 C# 源文件、Properties、app.ico、app.manifest 和名为 `-` 的嵌入资源放入本地工程，保留目录结构。GameDir 指向包含项目引用 DLL 的游戏目录。

```sh
dotnet build Shenzhen.csproj -p:GameDir="/path/to/game/assemblies"
```

公开包仅提供工程配置；游戏依赖、源码和资源由使用者在本地提供。
