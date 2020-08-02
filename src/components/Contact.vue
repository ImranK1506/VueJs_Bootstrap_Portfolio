<template>
  <div>
    <div class="container" style="padding:10%">
      <h2>Contact Me</h2>
      <form action="mailto:info@yourdutchdev.com"
            method="post"
            enctype="text/plain">
        <div class="form-group">
          <input type="email"
                 class="form-control"
                 v-model="contact.email"
                 placeholder="Enter email">
        </div>
        <div class="form-group">
              <textarea class="form-control"
                        v-model="contact.message"
                        rows="3"
                        placeholder="write message">
              </textarea>
        </div>
      </form>
      <div class="modal-footer">
        <button type="button"
                data-dismiss="modal"
                class="btn btn-danger btn-lg"
        >Go back
        </button>
        <button type="button"
                @click="submit"
                class="btn btn-dark btn-lg"
        >Reach out
        </button>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: "Contact",
  data() {
    return {
      contact: {
        email: '',
        message: ''
      }
    }
  },
  methods: {
    submit() {
      // Form validation
      if (this.contact.email != '' && this.contact.message != '') {
        //  send details
      } else {
        alert('All fields are required');
      }
    }
  }
}

</script>

<style scoped>

</style>