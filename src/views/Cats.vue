<template>
  <div>
    <PetTable species="cats" :pets="cats"></PetTable>
  </div>
</template>

<script>
import { mapState } from "vuex";
import PetTable from "@/components/PetTable.vue";
export default {
  components: {
    PetTable
  },
  data() {
    return {};
  },
  computed: {
    //takes the part of vuex state you want
    ...mapState(["cats"])
  }
};
</script>

