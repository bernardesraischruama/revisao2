<script>
export default {
    name: 'EquipeView',
    data() {
        return {
            equipe: [
                {
                    nome: 'Juliane',
                    cargo: 'Desenvolvedor'
                },
                {
                    nome: 'Ruama',
                    cargo: 'Designer'
                },
                {
                    nome: 'Ester',
                    cargo: 'Gerente de Projetos'
                }
            ]
        }
    }
}
</script>

<template>
    <div>
        <h1>Equipe</h1>
        <ul>
            <li v-for="membro in equipe" :key="membro.nome">
                <h2>{{ membro.nome }}</h2>
                <p>{{ membro.cargo }}</p>
            </li>
        </ul>
    </div>
</template>

<style scoped>
/* Your component-specific styles go here */
</style>