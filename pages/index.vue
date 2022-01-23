<template>
<v-form>
  <v-row justify="center" align="center">
    <v-col cols="12"
      sm="10"
      md="8"
      lg="6">
      <v-card class="logo py-4 d-flex justify-center">
        <v-img
        height="300"
        src="https://assurecondo.com/wp-content/uploads/2021/07/smart-contract-1-900x313.png"
        ></v-img>
      </v-card>
      <v-card ref="form">
        <v-card-title class="justify-center" style="font-size:2em" >Employee Form</v-card-title>
        <v-card-text>
          <v-text-field
            ref="name"
            v-model="first"
            label="ETH Price"
            outline
            readonly
          ></v-text-field>
          <v-text-field
            ref="address"
            v-model="second"
            label="ETH Blocked"
            readonly
            disabled
            ></v-text-field>
          <v-text-field
            ref="city"
            v-model="third"
            label="Project Cost (ETH)"
            readonly
            ></v-text-field>
          <v-text-field
            ref="state"
            v-model="fourth"
            label="Project Cost"
            readonly
            ></v-text-field>
          <v-text-field
            ref="zip"
            v-model="fifth"
            label="Contractor Public Key"
            readonly
            ></v-text-field>
         </v-card-text>
         <v-card-actions>
         <div class="my-2">
          <v-btn
          color="primary"
          light
          background-color="yellow">
            Project Start
          </v-btn>
          </div>
          <v-spacer></v-spacer>
          <v-btn
            color="orange"
            light
            bold
            @click="submit"
          >
            Submit
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
 </v-form>
</template>
<script>
  export default {
    data: () => ({
      first: "$ 2495",
      second: "$ 0,1",
      third: "$ 0,80",
      fourth: "$ 2000",
      fifth: "0x563FE49697B9eec5cd2F701047dEa4221caF0402"
    }),

  }
</script>
