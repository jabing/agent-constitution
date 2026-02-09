## ✅ 修改完成报告

### 📋 修改概要
- **方案**: Option 1 - 只替换不合适的两个人物
- **替换内容**:
  - 诸葛亮 → 商鞅 (Shang Yang)
  - 曾国藩 → 韩非子 (Han Feizi)
- **保持不变**: 司马迁、鲁班、包拯、张衡

### 📁 修改文件列表 (8个)
#### 主文件 (4个):
1. ✅ agents/planner.md
2. ✅ governance/CONDUCTOR.md  
3. ✅ governance/AGENT_CONSTITUTION.md
4. ✅ docs/PERSONA_PROFILES.md

#### Vendor副本 (4个):
5. ✅ vendor/agent-constitution/agents/planner.md
6. ✅ vendor/agent-constitution/governance/CONDUCTOR.md
7. ✅ vendor/agent-constitution/governance/AGENT_CONSTITUTION.md
8. ✅ vendor/agent-constitution/docs/PERSONA_PROFILES.md

### 🎯 具体修改内容
#### 商鞅 (Planner):
- **标题**: 任务定界官 → 法令制定官
- **人格锚点**: 
  - 克制的全局视角 → 法令明确性
  - 极强的边界意识 → 边界不可协商  
  - 对"模糊命令"的天然警惕 → 执行可验证性
- **System Prompt**: Persona anchor: Shang Yang

#### 韩非子 (CONDUCTOR):
- **标题**: 终局裁决协议（移除人物符号）
- **人格锚点**:
  - ≠ 智谋型 → ≠ 仁慈型
  - ≠ 执行型 → ≠ 协商型
  - 收口者/裁决者/自我克制者 → 法家裁决者/制度终结者/冷酷终局者
- **System Prompt**: Persona anchor: Han Feizi
- **对齐说明**: 移除 Chinese-Persona System 标签

#### 宪法更新:
- **角色总览表**: 更新两人引用
- **权力流向图**: 更新流程图人物标注

#### 人物小传更新:
- **商鞅章节**: 重写核心描述，强调"法令制定"特性
- **韩非子章节**: 重写核心描述，强调"法家裁决"特性
- **使用顺序**: 更新为 司马迁→商鞅→鲁班→包拯→张衡→韩非子

### ✅ 验证结果
1. **主文件清理**: ✅ 无诸葛亮、曾国藩残留引用
2. **新引用统计**: ✅ vendor目录中21处商鞅/韩非子引用
3. **Setup测试**: ✅ `node setup-opencode.js --force` 成功运行
4. **OpenCode显示**: ✅ 只显示角色功能描述，不显示人物名
5. **vendor同步**: ✅ 所有副本文件同步更新

### 🎯 实现目标
- ✅ **功能匹配提升**: 商鞅/韩非子更符合角色约束本质
- ✅ **保持简洁**: OpenCode界面仍只显示功能描述
- ✅ **风险控制**: 历史人物无版权问题
- ✅ **文化延续**: 保持中国历史人物主题
- ✅ **最小改动**: 只替换问题最明显的两个人物

### 📝 备注说明
- 人物锚点仅作为教育隐喻，不影响Agent实际执行
- OpenCode界面显示的角色功能描述未改变
- 所有角色约束和宪法机制保持不变
- setup-opencode.js 生成文件正常工作

---
**修改完成时间**: 2026-02-08 16:45:59
