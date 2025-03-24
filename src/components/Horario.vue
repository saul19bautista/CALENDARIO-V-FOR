<template>
    <div class="container">
        <h3 class="mt-4 text-center">Horario de clases de Sistemas</h3>
        <table class="table table-striped table-bordered">
            <thead class="table-dark text-center">
                <tr>
                    <th scope="col">#</th>
                    <th scope="col">Horario</th>
                    <th scope="col">Lunes</th>
                    <th scope="col">Martes</th>
                    <th scope="col">Miércoles</th>
                    <th scope="col">Jueves</th>
                    <th scope="col">Viernes</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(h, index) in horario" :key="index">
                    <td>{{ index + 1 }}</td>
                    <td>{{ h.hora }}</td>
                    <td>{{ h.lunes}}</td>
                    <td>{{ h.martes}}</td>
                    <td>{{ h.miercoles}}</td>
                    <td>{{ h.jueves}}</td>
                    <td>{{ h.viernes}}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const horario = ref([
    { hora: '7:00-9:00', lunes: 'Programación Lógica y Funcional', martes: 'Inteligencia Artificial', miercoles: 'Desarrollo Agil', jueves: 'Programacion Logica Y Funcional', viernes: '' },
    { hora: '9:00-11:00', lunes: 'Desarrollo Agil', martes: 'Administracion De Redes ', miercoles: '', jueves: 'Administracion De Redes', viernes: '' },
    { hora: '10:00-11:00', lunes: '', martes: ' ', miercoles: '', jueves: '', viernes: 'Desarrollo Agil' },
    { hora: '11:00-1:00', lunes: '', martes: 'Desarrollo En La Nube', miercoles: 'Desarrollo En La Nube', jueves: 'Inteligencia Artificial', viernes: '' },
    { hora: '11:00-12:00', lunes: '', martes: ' ', miercoles: '', jueves: '', viernes: 'Desarrollo en la nube' },
    { hora: '1:00-2:00', lunes: '', martes: '', miercoles: '', jueves: 'Desarrollo Con Realidad Aumentada', viernes: '' },
    { hora: '1:00-3:00', lunes: '', martes: '', miercoles: 'Desarrollo Con Realidad Aumentada', jueves: '', viernes: '' },
    { hora: '2:00-4:00', lunes: '', martes: '', miercoles: '', jueves: '', viernes: 'Taller De Investigacion II' },
    { hora: '3:00-5:00', lunes: '', martes: 'Desarrollo Con Realidad Aumentada', miercoles: 'Taller De Investigacion II', jueves: '', viernes: '' },
    
]);
</script>
