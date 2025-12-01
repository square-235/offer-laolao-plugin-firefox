# Chrome扩展转Firefox扩展修改计划

## 1. 修改manifest.json配置
- 将`manifest_version`从3改为2（Firefox对v3支持不完全）
- 修改background配置，使用`scripts`而非`service_worker`
- 调整权限声明，确保Firefox支持
- 移除或调整`content_security_policy`配置

## 2. 调整background.js
- 确保使用的API在Firefox中可用
- 调整事件监听器实现

## 3. 检查content.js
- 确保API调用与Firefox兼容
- 调整事件处理逻辑

## 4. 验证popup相关文件
- 确保HTML和JavaScript代码在Firefox中正常运行
- 调整API调用确保兼容性

## 5. 测试和验证
- 确保扩展在Firefox中能正常加载和运行
- 测试核心功能是否正常工作

## 修改步骤
1. 首先修改manifest.json，这是最关键的一步
2. 然后检查并修改background.js
3. 接着检查content.js
4. 最后验证popup相关文件
5. 进行测试和调试

通过以上修改，将Chrome扩展转换为兼容Firefox的扩展。