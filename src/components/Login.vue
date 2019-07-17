<<template>
    <div class="login-form">
    </div>
</template>

<script lang="ts">
import Vue from 'vue'

import { LOGIN_REQUEST } from '@/store/actions'

export default Vue.extend({
  name: 'Login',
  data: () => ({
    username: String,
    password: String,
  }),
  methods: {
    async login(): Promise<void> {
      this.$store.dispatch(LOGIN_REQUEST)
    },
  },
})
</script>
