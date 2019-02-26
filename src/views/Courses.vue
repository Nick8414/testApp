<template>
  <div>
    <h1>This is an courses page</h1>
    <Table
      :data = "data"
      :columns = "columns"></Table>
  </div>
</template>

<script>
import Table from '@/components/Table.vue'
export default {
  components : {
    Table
  },
  data() {
    return {
      columns: ['name', 'eMail', 'status', 'action' ],
      data: [ {
                name: 'Gary Busey',
                eMail: 'busey@mail.com',
                status: 'active',
                action: ''
              },
              {
                name: 'Jeff Bridges',
                eMail: 'bridges@mail.com',
                status: 'active',
                action: ''
              },
              {
                name: 'Roger Corman',
                eMail: 'corman@mail.com',
                status: 'active',
                action: ''
              },
            ]
    }
    }
  
}
</script>
<style>

</style>



