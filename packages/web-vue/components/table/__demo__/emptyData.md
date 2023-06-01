```yaml
title:
  zh-CN: 空数据
  en-US: Basic Usage
```

## zh-CN

测试

---

## en-US

For the basic usage of the table, you need to pass `columns` and `data`.

---

```vue
<template>
  <!-- <a-table :columns="columns" :data="data" :scroll="data.length ? { x: 1400, y: `200px` } : {}" /> -->
  <a-table :columns="columns" :data="data" :scroll="{ x: 1400, y: `200px` }"/>
  <a-table :columns="columns" :data="data" />
</template>

<script>
import { reactive } from 'vue';

export default {
  setup() {
    const columns = [
      // 表格的列名等信息
      {
        title: '实验流水号',
        dataIndex: 'exp_code',
        slotName: 'exp_code',
        fixed: 'left',
        width: 110,
      },
      {
        title: '检测项目',
        dataIndex: 'product_name',
        slotName: 'product_name',
        fixed: 'left',
        width: 200,
      },
      {
        title: '样本条码',
        dataIndex: 'sample_barcode',
        slotName: 'sample_barcode',
        width: 140,
      },
      {
        title: '姓名',
        dataIndex: 'examinate_name',
        width: 70,
      },
      {
        title: '性别',
        dataIndex: 'sex',
        width: 50,
      },
      {
        title: '年龄',
        dataIndex: 'age',
        width: 50
      },
      {
        title: '联系电话',
        dataIndex: 'phone',
        width: 110,
      },
      {
        title: '临床诊断',
        dataIndex: 'clinic_history',
        width: 160,
      },
      {
        title: '交接单号',
        dataIndex: 'receive_code',
        slotName: 'receive_code',
        width: 120,
      },
      {
        title: '收样时间',
        dataIndex: 'receive_time',
        width: 160,
      },
      {
        title: '检测时间',
        dataIndex: 'check_time',
        width: 160,
      },
      {
        title: '初审时间',
        dataIndex: 'preliminary_time',
        width: 160,
      },
      {
        title: '复审时间',
        dataIndex: 'report_time',
        width: 160,
      },
      {
        title: '退单时间',
        dataIndex: 'chargeback_time',
        width: 160,
      },
      {
        title: '退单原因',
        dataIndex: 'chargeback_reason',
        width: 160,
      },
      {
        title: '备注',
        dataIndex: 'exp_remarks',
        slotName: 'exp_remarks',
        width: 160,
      },
      {
        title: '操作',
        dataIndex: 'operation',
        slotName: 'operation',
        fixed: 'right',
        width: 140,
      },
    ];
    // const columns = [
    //   {
    //     title: 'Name',
    //     dataIndex: 'name',
    //   },
    //   {
    //     title: 'Salary',
    //     dataIndex: 'salary',
    //   },
    //   {
    //     title: 'Address',
    //     dataIndex: 'address',
    //   },
    //   {
    //     title: 'Email',
    //     dataIndex: 'email',
    //   },
    //    {
    //     title: 'test1',
    //     dataIndex: 'test1',
    //   },
    //   {
    //     title: 'test2',
    //     dataIndex: 'test2',
    //   },
    //   {
    //     title: 'test3',
    //     dataIndex: 'test3',
    //   },
    //   {
    //     title: 'test4',
    //     dataIndex: 'test4',
    //   },
    //   {
    //     title: 'test5',
    //     dataIndex: 'test5',
    //   },
    //   {
    //     title: 'test6',
    //     dataIndex: 'test6',
    //   },
    //   {
    //     title: 'test7',
    //     dataIndex: 'test7',
    //   },
    //   {
    //     title: 'test8',
    //     dataIndex: 'test8',
    //   },
    //   {
    //     title: 'test9',
    //     dataIndex: 'test9',
    //   },
    // ];
    const data = reactive([]);

    return {
      columns,
      data
    }
  },
}
</script>
```
