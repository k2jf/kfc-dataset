<template>
  <div class="dataset">
    <Card style="width:320px" class="kfc-card">
      <p class="title" slot="title">
        {{ title }}
      </p>
      <a
        href="#"
        slot="extra">
        <Dropdown>
          <Icon type="ios-more" />
          <DropdownMenu slot="list">
            <DropdownItem><a href="javascfipt: void(0)">重命名</a></DropdownItem>
            <DropdownItem><a href="javascfipt: void(0)">下载</a></DropdownItem>
            <DropdownItem><a href="javascfipt: void(0)">删除</a></DropdownItem>
            <DropdownItem><a href="javascfipt: void(0)">重试</a></DropdownItem>
          </DropdownMenu>
        </Dropdown>
      </a>
      <Row>
        <Col span="12">行数：68752</Col>
        <Col span="12">列数：123</Col>
      </Row>
      <Row>
        <Col span="24">时间范围：
        <Tooltip
          transfer
          content="2019-03-08 16:24:28"
          placement="top">
          2019-03-08
        </Tooltip>
        </Col>
        <Col span="24">创建时间：
        <Tooltip
          transfer
          content="2019-03-08 00:00:00 ~ 2017-03-09 23:59:59"
          placement="top"
          max-width="600">
          2017-03-08 ~ 2017-03-09
        </Tooltip>
        </Col>
      </Row>
    </Card>
  </div>
</template>
<script>
import { Icon, Card, Dropdown, DropdownMenu, DropdownItem, Row, Col, Tooltip } from 'iview'
export default {
  name: 'Dataset',
  components: {
    Icon,
    Card,
    Dropdown,
    DropdownMenu,
    DropdownItem,
    Row,
    Col,
    Tooltip
  },
  props: {
    title: {
      type: String,
      default: '数据集名称'
    }
  },
  data () {
    return {

    }
  }
}
</script>
<style scoped>
.dataset {
  display: inline-block;
}
.title {
  width: calc(100% - 30px);
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.dataset .ivu-col {
  line-height: 32px;
  height: 32px;
}
.ivu-tooltip-inner {
  max-width: 400px;
}
/* .dataset .kfc-card:hover {
  box-shadow: 1px 1px 6px rgb(68, 231, 177);
  cursor: pointer;
} */
</style>
