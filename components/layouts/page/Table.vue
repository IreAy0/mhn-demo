<template>
  <div class=" ">
    <!-- Tabs -->
    <div class="flex gap-2 ">
      <button
        class="px-12 py-4 rounded-t-xl text-[#088AD8] text-base font-medium bg-[#F2F4F7] "
      >
        Prescription Order
      </button>
      <button class="px-12 py-4 rounded-t-xl text-gray-500  bg-[#F2F4F7]">
        Dispensed
      </button>
    </div>

    <div class="bg-white  border-t">
   <!-- Search and Filter -->
   <div class="flex justify-between items-center px-4 py-3">
    <div class="flex items-center space-x-2">
      <div class="relative flex gap-1.5 items-center px-4 bg-[#F9FAFB] rounded-lg border">
        <span class="">
          <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M19.7552 18.5783L14.781 13.6041C16.1365 11.9463 16.803 9.83087 16.6425 7.69543C16.4821 5.55999 15.507 3.5679 13.919 2.13123C12.331 0.694554 10.2515 -0.0767949 8.1107 -0.0232684C5.96991 0.0302581 3.93158 0.904564 2.41734 2.41881C0.9031 3.93305 0.0287933 5.97137 -0.0247333 8.11216C-0.0782598 10.253 0.693089 12.3324 2.12976 13.9205C3.56644 15.5085 5.55852 16.4836 7.69397 16.644C9.82941 16.8044 11.9448 16.138 13.6027 14.7825L18.5768 19.7566C18.734 19.9084 18.9445 19.9924 19.163 19.9905C19.3815 19.9886 19.5905 19.901 19.745 19.7465C19.8995 19.592 19.9872 19.383 19.9891 19.1645C19.991 18.946 19.907 18.7355 19.7552 18.5783ZM8.33266 15.0008C7.01412 15.0008 5.72519 14.6098 4.62886 13.8773C3.53253 13.1447 2.67805 12.1035 2.17347 10.8854C1.66888 9.66718 1.53686 8.32673 1.79409 7.03353C2.05133 5.74032 2.68627 4.55243 3.61862 3.62008C4.55097 2.68773 5.73885 2.05279 7.03206 1.79556C8.32527 1.53832 9.66571 1.67035 10.8839 2.17493C12.1021 2.67952 13.1433 3.534 13.8758 4.63033C14.6083 5.72665 14.9993 7.01559 14.9993 8.33413C14.9973 10.1016 14.2943 11.7962 13.0445 13.046C11.7947 14.2958 10.1002 14.9988 8.33266 15.0008Z" fill="#98A2B3"/>
            </svg>
        </span>
       
          <input
          type="text"
          placeholder="Search"
          class="  py-2.5 w-[233px] bg-transparent  focus:outline-none"
        />
      </div>
    
      <button class="px-4 w-[99px] py-2 flex items-center text-base font-normal text-[#3F434A] justify-center gap-1.5 border rounded-lg"> 
        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M11.6672 20C11.4869 20 11.3115 19.9415 11.1672 19.8333L7.83389 17.3333C7.73039 17.2557 7.64639 17.1551 7.58853 17.0393C7.53067 16.9236 7.50055 16.796 7.50055 16.6667V11.9833L1.65389 5.40583C1.23865 4.9374 0.967536 4.35901 0.87312 3.7402C0.778704 3.12138 0.865007 2.48846 1.12166 1.91751C1.37831 1.34656 1.79438 0.861882 2.31987 0.521721C2.84536 0.181561 3.45791 0.000395349 4.08389 0L15.9172 0C16.5431 0.000734209 17.1555 0.182199 17.6808 0.522589C18.2061 0.862978 18.6219 1.34781 18.8783 1.91882C19.1347 2.48983 19.2207 3.12273 19.126 3.74146C19.0314 4.36018 18.7601 4.93841 18.3447 5.40667L12.5006 11.9833V19.1667C12.5006 19.3877 12.4128 19.5996 12.2565 19.7559C12.1002 19.9122 11.8882 20 11.6672 20ZM9.16722 16.25L10.8339 17.5V11.6667C10.8341 11.4626 10.9091 11.2657 11.0447 11.1133L17.1014 4.29917C17.3033 4.0709 17.4351 3.7892 17.4809 3.48788C17.5267 3.18655 17.4846 2.87842 17.3595 2.60046C17.2345 2.32251 17.0319 2.08655 16.7761 1.92091C16.5202 1.75527 16.222 1.66699 15.9172 1.66667H4.08389C3.77926 1.66713 3.48124 1.75546 3.22556 1.92105C2.96988 2.08665 2.76739 2.3225 2.64239 2.60029C2.51739 2.87809 2.47518 3.18605 2.52083 3.48723C2.56647 3.78842 2.69803 4.07004 2.89972 4.29833L8.95722 11.1133C9.09257 11.2659 9.16728 11.4627 9.16722 11.6667V16.25Z" fill="#667085"/>
          </svg>           
        Filter
      
      </button>
    </div>
  </div>

  <!-- Table -->
  <table class="min-w-full border-collapse table-auto text-left">
    <thead class="">
      <tr>
        <th class="p-3 border-b">
          <input type="checkbox" @change="toggleAll" v-model="selectAll" />
        </th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Date</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Order ID</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Patient Name</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Medications</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Admission Status</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Requested By</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Dispensed by</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Fee Status</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Service</th>
        <th class="p-3 border-b text-xs text-[#667085] font-medium">Actions</th>
      </tr>
    </thead>
    <tbody>
      <tr
        v-for="(item, index) in tableData"
        :key="index"
        class="text-sm"
      >
        <td class="p-3 border-b">
          <input type="checkbox" v-model="selected[index]" />
        </td>
        <td class="p-3 border-b">
          <p class="text-sm text-header5">{{ item.date }} </p> 
        <p class="text-sm text-header">{{item.time}}</p>
        </td>
        <td class="p-3 border-b text-[#3F434A]">{{ item.orderId }}</td>
        <td class="p-3 border-b text-[#3F434A]">{{ item.patientName }}</td>
        <td class="p-3 border-b">
          <a href="#" class="text-primary underline">{{ item.medications }}</a>
        </td>
        <td class="p-3 border-b">
          <span
            class="px-2 py-1 text-xs font-semibold rounded-full"
            :class="item.admissionStatus === 'Admitted'
              ? 'bg-green-100 text-green-600'
              : ''"
          >
            {{ item.admissionStatus }}
          </span>
        </td>
        <td class="p-3 border-b text-[#3F434A]">{{ item.requestedBy }}</td>
        <td class="p-3 border-b">-</td>
        <td class="p-3 border-b">
          <span
            class="px-2 py-1 text-xs font-semibold rounded-full"
            :class="item.feeStatus === 'Paid'
              ? 'bg-green-100 text-green-600'
              : 'bg-blue-100 text-blue-600'"
          >
            {{ item.feeStatus }}
          </span>
        </td>
        <td class="p-3 border-b">
          <span
            class="px-2 py-1 text-xs font-semibold rounded-full bg-yellow-100 text-yellow-600"
          >
            {{ item.service }}
          </span>
        </td>
        <td class="p-3 border-b">
          <button class="text-gray-600">⋮</button>
        </td>
      </tr>
    </tbody>
  </table>
    </div>
 
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectAll: false,
      selected: {},
      tableData: [
        {
          time:'3:45 PM',
          date: '04/06/2024 5:45 PM',
          orderId: 'PRE001',
          patientName: 'Durosinmi Jolayemi',
          medications: 3,
          admissionStatus: 'Admitted',
          requestedBy: 'Dr. Moses Dele',
          feeStatus: 'Paid',
          service: 'Pending',
        },
        {
          time:'3:45 PM',
          date: '04/06/2024 ',
          orderId: 'PRE001',
          patientName: 'Olaide Chika',
          medications: 1,
          admissionStatus: 'Admitted',
          requestedBy: 'Dr. Moses Dele',
          feeStatus: 'Billed',
          service: 'Pending',
        },
      ],
    };
  },
  methods: {
    toggleAll() {
      this.tableData.forEach((item, index) => {
        this.$set(this.selected, index, this.selectAll);
      });
    },
  },
  watch: {
    selected: {
      deep: true,
      handler(newVal) {
        this.selectAll =
          Object.keys(newVal).length > 0 &&
          Object.values(newVal).every((selected) => selected);
      },
    },
  },
};
</script>

<style scoped>
/* Add custom styles here if needed */
</style>
