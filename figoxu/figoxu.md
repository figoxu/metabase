
## 开发环境

IDEA安装Cursive的插件

## 运维扩展

https://www.yuque.com/leryn/wiki/toolchain.metabase

helm add repo infra harbor.mydomain.com/infra/chartrepo
helm pull infra/metabase

helm install metabase stable/metabase -n metabase \
--set database.dbname=metabase \
--set database.host=xxx.xxx.xxx.xxx \
--set database.password=xxxxxxxxx \
--set database.port=3306 \
--set database.type=mysql \
--set database.username=metabase \
--set image.repository=harbor.mydomain.com/infra/metabase \
--set image.tag=v0.44.5 \
--set ingress.enabled=true \
--set ingress.hosts={metabase.mydomain.com} \
--set timeZone=Asia/Shanghai

## 目录概述
Metabase是一个开源的业务智能工具，用于帮助用户可视化和理解数据。根据你提供的目录结构，下面是每个目录可能的作用：

1. `bin`: 包含可执行文件或脚本，可能是启动Metabase服务、管理数据库连接或其他命令行工具。

2. `dev`: 开发相关文件，可能包含开发文档、脚本、配置或开发工具。

3. `docs`: 存放项目文档，包括API文档、开发指南、用户手册等。

4. `e2e`: 端到端测试相关文件，用于自动化测试整个应用的流程。

5. `enterprise`: 企业版Metabase的特定文件，可能包含额外的付费功能、插件或定制代码。

6. `frontend`: 前端代码，包括用户界面、样式表、JavaScript等。

7. `hooks`: 可能包含Git钩子脚本，用于自动化执行某些任务，如代码检查、测试等。

8. `locales`: 本地化文件，包含不同语言的翻译资源，用于支持多语言界面。

9. `modules`: 可能包含可复用的模块或插件，用于扩展Metabase的功能。

10. `patches`: 包含补丁文件，可能是对Metabase代码的临时修改或修复。

11. `release`: 发布相关文件，可能包含构建脚本、版本信息、发布说明等。

12. `resources`: 可能包含与Metabase相关的资源文件，如图标、图片或其他媒体文件。

13. `snowplow`: Snowplow是一个开源的事件收集平台，这个目录可能包含与Metabase集成的Snowplow相关代码。

14. `src`: 主要源代码目录，存放Metabase的核心代码。

15. `test`: 单元测试或集成测试代码，用于验证Metabase的功能。

16. `test_config`: 测试环境的配置文件。

17. `test_modules`: 测试模块，可能包含用于测试目的的特定代码或脚本。

18. `test_resources`: 测试资源文件，如测试用的数据库文件、配置文件等。

请注意，这些解释是基于目录名称的一般理解，具体项目中每个目录的实际内容和用途可能会有所不同。如果需要更精确的信息，建议查看Metabase的官方文档或源代码仓库中的相关说明。
