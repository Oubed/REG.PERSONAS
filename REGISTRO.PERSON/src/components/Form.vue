<template>
  <form >
    <div class="grid grid-cols-3 gap-4">
      <div  class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="nombre">
        Nombre
      </label>
      <input v-model="nombre" class="shadow appearance-none border rounded w-150 py-2 px-6 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="nombre" type="text" placeholder="nombre">
    </div>
      <div  class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="edad">
        Edad
      </label>
      <input v-model="edad" class="shadow appearance-none border rounded w-150 py-2 px-6 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="edad" type="number" placeholder="">
    </div>

    <div class="mb-4">
    <label class="block text-gray-700 text-sm font-bold mb-2" for="estado">
        Estado Civil
    </label>
      <select v-model="estadoCivil" class="block appearance-none w-full bg-white border border-gray-400 hover:border-gray-500 px-4 py-2 pr-8 rounded shadow leading-tight focus:outline-none focus:shadow-outline">
      <option value="1">1. Soltero</option>
      <option value="2">2. Casado</option>
      <option value="3">3. Divorsiado</option>
      <option value="4">4. Separado</option>
      <option value="5">5. Union libre</option>
      <option value="6">6. Viudo</option>
      </select>
    </div>


    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="trabajo">
        Trabajo
      </label>
      <input v-model="trabajo" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="trabajo" placeholder="trabajo">
    </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="residencia">
        Residencia
      </label>
      <input v-model="residencia" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="residencia" placeholder="residencia">
    </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="cita">
        Cita
      </label>
      <input v-model="cita" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="text" placeholder="cita">
    </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="citaautor">
        Cita Autor
      </label>
      <input v-model="citaAutor" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="text" placeholder="cita autor">
    </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="bio">
        Biografia
      </label>
      <input v-model="bio" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="text" placeholder="">
    </div>

    

    <div class="mb-4">
            <label
              for="per01"
              class="block mb-2  font-medium text-gray-900  mb-4">personalidad 1</label>
            <input
              v-model="personalidad01"
              type="range"
              min="0"
              max="100"
              class="mt-1 block w-full border-none bg-gray-100 h-11 rounded-xl shadow-lg hover:bg-blue-100 focus:bg-blue-100 focus:ring-0"
              
              />
              <span>{{ this.personalidad01 }}%</span>
          </div>

          <div class="mb-4">
            <label
              for="per02"
              class="block mb-2  font-medium text-gray-900  mb-4"
              >personalidad 2</label
            >
            <input
              v-model="personalidad02"
              type="range"
              min="0"
              max="100"
              class="mt-1 block w-full border-none bg-gray-100 h-11 rounded-xl shadow-lg hover:bg-blue-100 focus:bg-blue-100 focus:ring-0"
              
              />
              <span>{{ this.personalidad02 }}%</span>
          </div>

          <div class="mb-4">
            <label
              for="per03"
              class="block mb-2  font-medium text-gray-900  mb-4"
              >personalidad 3</label
            >
            <input
              v-model="personalidad03"
              type="range"
              min="0"
              max="100"
              class="mt-1 block w-full border-none bg-gray-100 h-11 rounded-xl shadow-lg hover:bg-blue-100 focus:bg-blue-100 focus:ring-0"
              
              />
              <span>{{ this.personalidad03 }}%</span>
          </div>

          <div class="mb-4">
            <label
              for="per04"
              class="block mb-2  font-medium text-gray-900  mb-4"
              >personalidad 4</label
            >
            <input
              v-model="personalidad04"
              type="range"
              min="0"
              max="100"
              class="mt-1 block w-full border-none bg-gray-100 h-11 rounded-xl shadow-lg hover:bg-blue-100 focus:bg-blue-100 focus:ring-0"
              
              />
              <span>{{ this.personalidad04 }}%</span>
          </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="obj">
        Objetivos
      </label>
      <input v-model="objetivos" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="text" placeholder="">
    </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="frus">
        Frustraciones
      </label>
      <input v-model="frustraciones" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="text" placeholder="">
    </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="motiv">
        Motivaciones
      </label>
      <input v-model="motivaciones" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="text" placeholder="">
    </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="marcas">
        Marcas
      </label>
      <input v-model="marcas" class="shadow appearance-none border rounded w-150 py-2 px-6 text-blue-700 leading-tight focus:outline-none focus:shadow-outline" id="string" type="text" placeholder="">
    
    </div>
      <button @click="enviar()" class="bg-blue-500 hover:bg-blue-700 rounded w-25 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="button">
        Enviar
      </button>
    </div>
  </form>
</template>

<script>
import axios from 'axios'
export default {
  data(){
return{
  nombre: "",
  edad: "",
  estadoCivil: "",
  trabajo: "",
  residencia: "",
  cita: "",
  citaAutor: "",
  bio: "",
  personalidad01: "0",
  personalidad02: "0",
  personalidad03: "0",
  personalidad04: "0",
  objetivos: "",
  frustraciones:"",
  motivaciones: "",
  marcas: "",
};
  },
  methods:{
    enviar() {
      axios
.post("/api/guardarPersonasUxd.php", {
nombre: this.nombre,
edad: this.edad,
estadoCivil: this.estadoCivil,
trabajo: this.trabajo,
residencia: this.residencia,
cita: this.cita,
citaAutor: this.citaAutor,
bio: this.bio,
personalidad01: this.personalidad01,
personalidad02: this.personalidad02,
personalidad03: this.personalidad03,
personalidad04: this.personalidad04,
objetivos:this.objetivos,
frustraciones: this.frustraciones,
motivaciones: this.motivaciones,
marcas: this.marcas,
//completar las variables, estas deben llamarse como las que se recibirán en el backend sin el símbolo del dolar $
})
.then((response) => {
console.log(response.status)
});
}
}
  
}
</script>

<style>
</style>
