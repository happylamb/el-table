<template>
  <div class="my-table">
    <el-table :data="rows">
      <el-table-column
              prop="key1">
        <template slot-scope="scope" slot="header">
          <div class="block">
            <el-date-picker
                    v-model="value1"
                    type="datetimerange"
                    start-placeholder="开始日期"
                    end-placeholder="结束日期"
                    value-format="yyyy-MM-dd HH:mm:ss"
                    @change="timeChangeAction"
                    :default-time="['12:00:00']">
            </el-date-picker>
          </div>
        </template>
      </el-table-column>
      <el-table-column
              label="key2"
              prop="key2">
      </el-table-column>
      <el-table-column
              label="key3"
              prop="key3">
      </el-table-column>
      <el-table-column
              label="key4"
              prop="key4">
      </el-table-column>


    </el-table>

  </div>
</template>


<script>
  export default {
    name: 'Home',
    data(){
      return{
        value1:'',
        rows:[
          {key1:'111', key2:'222',key3:'333',key4:'444'},
          {key1:'111as', key2:'22221',key3:'343',key4:'434'},
          {key1:'111f', key2:'fd222',key3:'hgh333',key4:'ccx444'},
        ]
      }
    },
    methods:{
      timeChangeAction(){
        console.log(this.value1);
      }
    }
  }
</script>
