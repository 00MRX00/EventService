<template>
    <div>
        <h1>Logout</h1>
    </div>
</template>

<script>
import { mapActions } from "vuex";

export default {
    beforeMount() {
        this.logout()
        this.$router.push('/')
	},
    methods: {
		...mapActions(["logout"]),
	}
}
</script>