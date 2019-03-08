<template>
  <div>
    <div>
      <label>
        Full Name :
        <input
          type="text"
          class="contact-input"
          v-model="formData.fullName">
      </label>
    </div>
    <div>
      <label>
        Email :
        <input
          type="email"
          v-model="formData.email">
      </label>
    </div>
    <div>
      <label>
        Description :
        <textarea v-model="formData.description"></textarea>
      </label>
    </div>
    <div>
      <button>Submit</button>
    </div>
    <div>
      {{formData}}
    </div>
  </div>
</template>

<script type="text/javascript">
  export default {
    name: 'ContactUsPage',
    data () {
      return {
        formData: {
          fullName: '',
          email : '',
          description : ''
        }
      }
    }
  }
</script>

<style scoped>
  label {
    display: block;
    padding-top: 10px;
  }
</style>
