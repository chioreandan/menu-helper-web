<template>
  <b-form>
    <b-row class="justify-content-center mt-5">
      <b-col cols="4">
        <b-form-group label="Email"
          label-size="lg"
          label-class="font-weight-bold text-left pt-0">
          <b-form-input placeholder="Email" v-model="email"/>
        </b-form-group>
      </b-col>
    </b-row>
    <b-row class="mt-2 justify-content-center">
      <b-col cols="4">
        <b-form-group label="Password"
          label-size="lg"
          label-class="font-weight-bold text-left pt-0">
          <b-form-input placeholder="Password" v-model="password"/>
        </b-form-group>
      </b-col>
    </b-row>
    <b-row class="mt-2 justify-content-center">
      <b-col cols='2'>
        <b-button block variant="primary font-weight-bold"> Login </b-button>
      </b-col>
    </b-row>
  </b-form>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class LoginForm extends Vue {
  email = '';

  password = '';
}
</script>
