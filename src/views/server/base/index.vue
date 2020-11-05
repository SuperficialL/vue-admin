<template>
  <div>
    <div class="header">
      <el-button type="success" size="mini">启动监控服务</el-button>
      <el-button type="danger" size="mini">停止监控服务</el-button>
    </div>
    <el-table
      :data="table"
      border
      style="width: 100%"
    >
      <el-table-column
        label="服务名称"
        width="180"
        align="center"
      />
      <el-table-column
        label="描述"
        width="180"
        align="center"
      />
      <el-table-column
        label="状态"
        align="center"
      />
      <el-table-column
        label="操作"
        align="center"
      />
    </el-table>
  </div>
</template>

<script>
export default {
  name: 'Base',
  data() {
    return {
      table: []
    }
  }
}
</script>

<style lang="scss" scoped>
.header {
  padding: 10px 20px;
}
</style>
