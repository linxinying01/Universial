BigWorldEngine/
├── Build/                   # 构建系统配置
│   ├── Windows/
│   ├── Linux/
│   └── CMakeLists.txt
├── Docs/                    # 设计文档
│   ├── NetworkProtocol.md
│   └── EntitySystem.md
├── Engine/                  # 引擎核心
│   ├── Core/                # 基础框架
│   │   ├── Memory/          # 内存管理
│   │   ├── Math/            # 数学库
│   │   └── Utils/           # 通用工具
│   ├── ECS/                 # 实体组件系统
│   │   ├── EntityManager.cpp
│   │   ├── ComponentPool.h
│   │   └── Systems/
│   ├── Scene/               # 场景管理
│   │   ├── ChunkStreaming/
│   │   ├── SpatialPartition/ # 空间划分
│   │   └── LOD/
│   ├── Network/             # 网络模块
│   │   ├── Protocol/        # 协议定义
│   │   ├── AOI/             # 兴趣区域管理
│   │   └── RPC/
│   ├── Resources/           # 资源管理
│   │   ├── Loaders/         # 资源加载器
│   │   ├── HotReload/       # 热更新系统
│   │   └── AssetPipeline/  # 资源处理管线
│   └── Rendering/           # 渲染模块
│       ├── VulkanBackend/
│       ├── Shaders/
│       └── GPUScene/
├── Server/                  # 服务器架构
│   ├── Gateway/             # 网关服务器
│   ├── SceneServer/         # 场景服务器
│   ├── Central/             # 中心服务器
│   └── Shared/              # 服务器公共代码
├── Tools/                   # 开发工具链
│   ├── WorldEditor/         # 场景编辑器
│   │   ├── TerrainSculpting/
│   │   └── VegetationPainting/
│   ├── BehaviorTreeEditor/  # 行为树编辑器
│   ├── Profiler/            # 性能分析器
│   └── AssetBaker/          # 资源烘焙工具
├── ThirdParty/              # 第三方库
│   ├── entt/                # ECS库
│   ├── lz4/                 # 压缩库
│   └── recastnavigation/   # 寻路库
├── Tests/                   # 自动化测试
│   ├── UnitTests/           # 单元测试
│   └── StressTests/         # 压力测试
├── Samples/                 # 示例项目
│   ├── DemoGame/            # 演示游戏
│   └── Scripts/             # Lua/Python示例
└── Scripts/                 # 构建/部署脚本
    ├── CI/                  # 持续集成
    └── Deployment/          # 部署脚本