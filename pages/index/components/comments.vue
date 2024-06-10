<template>
    <div v-if="visible" class="comment-card">
        <v-card>
            <v-card-item>
                <v-card-title>{{ nombredeusuario }}</v-card-title>
                <v-card-text>{{ comentario }}</v-card-text>
                <v-btn>Comentar</v-btn>
            </v-card-item>
        </v-card>
    </div>
</template>
<script>
export default {
  props: {
    nombredeusuario: String,
    comentario: String,
    visible: Boolean
  }
}
</script>
<style scoped>
.comment-card {
  margin-top: 8px;
  text-align: center;
}
</style>
