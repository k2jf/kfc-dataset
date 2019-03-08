## kfc-dataset

> author: kk

## 使用
```
# 安装依赖
npm install kfc-dataset
# 克隆组件到当前项目components中
git remote add -f kfc-dataset git@github.com:k2jf/kfc-dataset.git
git subtree add -P src/components/kfc-dataset kfc-dataset master --squash
# 检查一下是否成功连接远程库 kfc-dataset
git remote -vv
```

## 使用示例：
```vue
<template>
  <Dataset />
</template>
<script>
import Dataset from '@/components/kfc-dataset'

export default {
  components: {
    Dataset
  }
}
</script>
```
