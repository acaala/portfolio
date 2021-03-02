<template>
  <div class="container mx-auto">
    <header class="flex justify-between mx-auto items-center py-4">
      <h1 class="title-font text-3xl primary-color">Liam Watts</h1>
      <nuxt-link to="/">
        <button class="btn-secondary">close</button>
      </nuxt-link>
    </header>

    <section class="my-12 container mx-auto">
      <h2 class="title-font text-3xl text-center text-white">Hi, Let's Talk</h2>

      <form
        @submit.prevent="sendMessage"
        class="flex flex-col container lg:w-1/2 md:w-2/3 mx-auto space-y-20 my-12"
      >
        <div class="flex flex-col">
          <label for="name" class="">Name</label>
          <input type="text" name="name" v-model="name" required />
        </div>
        <div class="flex flex-col">
          <label for="email">Email</label>
          <input type="email" name="email" v-model="email" required />
        </div>
        <div class="flex flex-col">
          <label for="message">Message </label>
          <textarea
            name="message"
            v-model="message"
            id="message"
            cols="30"
            rows="5"
            required
          ></textarea>
        </div>
        <div class="w-1/3 mx-auto flex justify-center">
          <button v-if="!loading" class="btn-primary w-full">Send</button>
          <div v-else class="spinner-box">
            <div class="configure-border-1">
              <div class="configure-core"></div>
            </div>
            <div class="configure-border-2">
              <div class="configure-core"></div>
            </div>
          </div>
        </div>
      </form>
    </section>
  </div>
</template>

<script lang="ts">
import {
  defineComponent,
  ref,
  onMounted,
  reactive,
} from '@nuxtjs/composition-api'

export default defineComponent({
  setup() {
    const name = ref('')
    const email = ref('')
    const message = ref('')
    let loading = ref(false)

    let form = reactive({
      from_name: name,
      from_email: email,
      message,
    })

    onMounted(() => {
      emailjs.init('user_TrkfR9PpcTKlsuGGOhD75')
    })

    const sendMessage = async () => {
      loading.value = true
      try {
        const response = await emailjs.send('gmail', 'portfolio', form)

        name.value = ''
        email.value = ''
        message.value = ''
        loading.value = false
        console.log(response)
      } catch (err) {
        console.log(err)
      }
    }

    return { name, email, message, sendMessage, loading }
  },
})
</script>
<style lang="postcss" scoped>
label {
  @apply leading-7 text-sm text-gray-400;
}

input,
textarea {
  outline: none;
  background: #a16ae8c4;
  border-bottom: 1px solid #4cfcd3;
  color: white;
  @apply px-3 rounded-sm py-1  transition-colors duration-200 ease-in-out;
}

input:focus,
textarea:focus {
  background-color: #a16ae8;
}

.configure-border-1 {
  width: 25px;
  height: 25px;
  padding: 3px;
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #fb5b53;
  animation: configure-clockwise 3s ease-in-out 0s infinite alternate;
}

.configure-border-2 {
  width: 25px;
  height: 25px;
  padding: 3px;
  left: -115px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: rgb(63, 249, 220);
  transform: rotate(45deg);
  animation: configure-xclockwise 3s ease-in-out 0s infinite alternate;
}

.configure-core {
  width: 100%;
  height: 100%;
  background-color: #a16ae8;
}

@keyframes configure-clockwise {
  0% {
    transform: rotate(0);
  }
  25% {
    transform: rotate(90deg);
  }
  50% {
    transform: rotate(180deg);
  }
  75% {
    transform: rotate(270deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

@keyframes configure-xclockwise {
  0% {
    transform: rotate(45deg);
  }
  25% {
    transform: rotate(-45deg);
  }
  50% {
    transform: rotate(-135deg);
  }
  75% {
    transform: rotate(-225deg);
  }
  100% {
    transform: rotate(-315deg);
  }
}
</style>>
