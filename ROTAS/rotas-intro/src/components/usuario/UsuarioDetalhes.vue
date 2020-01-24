<template>
	<div class="usuario-detalhe">
        <h3>Usuário Detalhes</h3>
        <p><strong>Código:</strong>&nbsp;{{ id }}</p>
        <!-- :to="`/usuario/${id}/editar`" -->
        <router-link tag="button" primario :to="{ 
            name: 'editarUsuario', 
            params: { id },
            query: { completo: false, lingua: 'pt-BR' }
        }">Editar</router-link>
        <br><br>
    </div>
</template>

<script>
export default {
	props: ['id'],
    /*
    data() {
        return {
            id: this.$route.params.id
        }
    },
    watch: {
        $route(to, from) {
            this.id = to.params.id
        }
    },
    */
}
</script>

<style>
	
</style>
