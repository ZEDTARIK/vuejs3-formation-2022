<template lang="">

    <table class="table table-hover">
        <thead>
            <th>#</th>
            <th>Full Name</th>
            <th></th>
        </thead>
        <tbody>
            <tr v-for="employee in Employees" :key="employee.id">
                <td> {{ employee.id }} </td>
                <td colspan="2"> {{ employee.FullName }}</td>
                <td></td>
            </tr>
        </tbody>
    </table>

</template>
<script>
export default {
    data() {
        return {
            Employees: [
                { id: 1, FullName: "Zouhair ETTARAK"},
                { id: 2, FullName: "Adam JOHN"},
                { id: 3, FullName: "Ariana GATTI"},
                { id: 4, FullName: "Claudio Albaness"}
            ]
        }
    },
}
</script>
<style lang="">
    
</style>