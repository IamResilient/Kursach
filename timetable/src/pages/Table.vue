<template>
<div>
  <q-table
    title="Table Title"
    :data="tableData"
    :columns="columns"
    row-key="name"
  />
</div>
</template>

<script>
export default {
  data: () => ({
    columns: [
      {
        name: 'desc',
        required: true,
        label: 'Dessert (100g serving)',
        align: 'left',
        field: 'name',
        sortable: true,
        classes: 'my-class',
        style: 'width: 500px'
      }
    ],
    tableData: [
      {
        name: 'Frozen Yogurt',
        calories: 159,
        fat: 6.0,
        carbs: 24,
        protein: 4.0,
        sodium: 87,
        calcium: '14%',
        iron: '1%'
      }
    ]
  })
}
</script>
