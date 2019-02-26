<template>
  <div>
    <h1>This is an courses page</h1>
    <n-Button>+</n-Button>
    <Table
      :data = "data"
      :columns = "columns"></Table>
      <n-modal></n-modal>
  </div>
</template>

<script>
import Table from '@/components/Table.vue'
import Button from '@/components/Button';
import Modal from '@/components/Modal';
export default {
  components : {
    Table,
    nButton: Button,
    nModal: Modal
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



