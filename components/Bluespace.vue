<template lang="">
    <div class="h-[440px] w-[100%] bg-no-repeat bg-cover mt-[23px] flex justify-between" style="background-image: url(bg_blue.png)">
        
        <div class="w-[420px] mt-[40px] ml-[40px]">

            <h1 class="text-[32px] text-white font-semibold ">An easy way to send requests to all suppliers</h1>
            <p class="text-white mt-[16px] text-[16px]">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt.</p>
        </div>
        <div class="w-[491px] h-[346px] bg-white rounded-[10px] mt-[30px] mr-[31px] mb-[44px]">
           <div class="pl-[20px] pr-[31px] pt-[22px] pb-[25px]">
               <h1 class="text-[20px] font-semibold">Send quote to suppliers</h1>
                <input type="text" value="What item you need?"  class="pl-[5px] border border-grey-400 text-[16px] font-normal rounded-[5px] w-[100%] h-[40px] mt-[18px] ">
                <input type="text" class="pl-[5px] border border-grey-400 rounded-[5px] w-[100%] h-[73px] mt-[20px] " placeholder="Type more details" >
                
                <div class="flex mt-[20px]">
                    <input type="text" value="Quantity" class="pl-[5px] border border-grey-400 rounded-[5px] w-[206px] h-[40px]  " placeholder="Type more details" >
                    <select name="" id="" class="pl-[5px] w-[111px] h-[40px] ml-[8px] border border-grey-400 rounded-[5px]">
                        <option value="Psc">Psc</option>
                    </select>
                </div>
                <button class="bg-blue-600 text-white py-[10.5px] px-[16px] rounded-[5px] mt-[20px]">Send inquiry</button>
           </div>

           

        </div>
    
    </div>
</template>
<script lang="ts" setup>
import { reactive, ref } from 'vue'
import type { FormInstance, FormRules } from 'element-plus'

const formSize = ref('default')
const ruleFormRef = ref<FormInstance>()
const ruleForm = reactive({
  name: 'Hello',
  region: '',
  count: '',
  date1: '',
  date2: '',
  delivery: false,
  type: [],
  resource: '',
  desc: '',
})

const rules = reactive<FormRules>({
  name: [
    { required: true, message: 'Please input Activity name', trigger: 'blur' },
    { min: 3, max: 5, message: 'Length should be 3 to 5', trigger: 'blur' },
  ],
  region: [
    {
      required: true,
      message: 'Please select Activity zone',
      trigger: 'change',
    },
  ],
  count: [
    {
      required: true,
      message: 'Please select Activity count',
      trigger: 'change',
    },
  ],
  date1: [
    {
      type: 'date',
      required: true,
      message: 'Please pick a date',
      trigger: 'change',
    },
  ],
  date2: [
    {
      type: 'date',
      required: true,
      message: 'Please pick a time',
      trigger: 'change',
    },
  ],
  type: [
    {
      type: 'array',
      required: true,
      message: 'Please select at least one activity type',
      trigger: 'change',
    },
  ],
  resource: [
    {
      required: true,
      message: 'Please select activity resource',
      trigger: 'change',
    },
  ],
  desc: [
    { required: true, message: 'Please input activity form', trigger: 'blur' },
  ],
})

const submitForm = async (formEl: FormInstance | undefined) => {
  if (!formEl) return
  await formEl.validate((valid, fields) => {
    if (valid) {
      console.log('submit!')
    } else {
      console.log('error submit!', fields)
    }
  })
}

const resetForm = (formEl: FormInstance | undefined) => {
  if (!formEl) return
  formEl.resetFields()
}

const options = Array.from({ length: 10000 }).map((_, idx) => ({
  value: `${idx + 1}`,
  label: `${idx + 1}`,
}))
</script>
<style lang="">
    
</style>