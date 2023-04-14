<script setup>
import { ref } from 'vue'

const nome = ref('')
const email = ref('')
const senha = ref('')
const senha01 = ref('')
const data = ref('')
const endereco = ref('')
const cidade = ref('')
const estado = ref('')
const hobbies = ref('')
const programacao = ref('')
const biografia = ref('')
const enviar = ref(false)
</script>

<template>
  <div class="formulario">
    <form @submit.prevent=" enviar = !enviar">
      <div>
        <p>DIGITE SEU NOME:</p>
        <input v-model="nome" placeholder="DIGITE SEU NOME" />

        <p>DIGITE SEU EMAIL:</p>
        <input v-model="email" placeholder="DIGITE SEU EMAIL" />

        <p>DIGITE SUA SENHA:</p>
        <input type="password" v-model="senha" placeholder="DIGITE SUA SENHA" />

        <p>CONFIRMAR SENHA:</p>
        <input type="password" v-model="senha01" placeholder="DIGITE SUA SENHA NOVAMENTE" />

        <p>DATA DE NASCIMENTO:</p>
        <input type="date" v-model="data">

        <p>DIGITE SEU ENDEREÇO:</p>
        <input type="text" v-model="endereco" placeholder="DIGITE SEU ENDEREÇO" />

        <p>DIGITE SUA CIDADE:</p>
        <input type="string" v-model="cidade" placeholder="DIGITE SUA CIDADE" />

        <P>ESTADO:</P>
        <select v-model="estado">
          <option value="AC">Acre</option>
          <option value="AL">Alagoas</option>
          <option value="AP">Amapá</option>
          <option value="AM">Amazonas</option>
          <option value="BA">Bahia</option>
          <option value="CE">Ceará</option>
          <option value="DF">Distrito Federal</option>
          <option value="ES">Espírito Santo</option>
          <option value="GO">Goiás</option>
          <option value="MA">Maranhão</option>
          <option value="MT">Mato Grosso</option>
          <option value="MS">Mato Grosso do Sul</option>
          <option value="MG">Minas Gerais</option>
          <option value="PA">Pará</option>
          <option value="PB">Paraíba</option>
          <option value="PR">Paraná</option>
          <option value="PE">Pernambuco</option>
          <option value="PI">Piauí</option>
          <option value="RJ">Rio de Janeiro</option>
          <option value="RN">Rio Grande do Norte</option>
          <option value="RS">Rio Grande do Sul</option>
          <option value="RO">Rondônia</option>
          <option value="RR">Roraima</option>
          <option value="SC">Santa Catarina</option>
          <option value="SP">São Paulo</option>
          <option value="SE">Sergipe</option>
          <option value="TO">Tocantins</option>
        </select>
        <p>DIGITE SEUS HOBBIES:</p>
        <input type="text" v-model="hobbies" placeholder="DIGITE SEUS HOBBIES" />

        <p>LINGUAGENS DE PROGRAMAÇÃO:</p>
        <input type="text" v-model="programacao" placeholder="DIGITE SUAS LINGUAGENS" />

        <p>BIOGRAFIA:</p>
        <textarea type="text" v-model="biografia" cols="30" rows="10"></textarea>

      </div>
      <button type="submit" >Salvar informações </button>
      <div v-if="enviar">
    <div> 
    <p>NOME:   {{ nome }}</p> 
    </div>
     <div> 
      <p>EMAIL:   {{ email }}</p> 
      </div>
      <div>
        <p>SENHA:   {{ senha}}</p> 
      </div>
      <div>
        <p>CONFIRMAR SENHA:   {{ senha01}}</p> 
      </div>
      <div>
        <p>DATA:   {{ data}}</p> 
      </div>
      <div>
        <p>ENDEREÇO:   {{ endereco}}</p> 
      </div>
      <div>
        <p>CIDADE:   {{ cidade}}</p> 
      </div>
      <div>
        <p>ESTADO:   {{ estado}}</p> 
      </div>
      <div>
        <p>HOBBIES:   {{ senha}}</p> 
      </div>
      <div>
        <p>LINGUAGENS:   {{ programacao}}</p> 
      </div>
      <div>
        <p>BIOGRAFIA:   {{ biografia}}</p> 
      </div>
      </div>
    </form>
  </div>
  
</template>




<style scoped>
.formulario {
  background-color: rgb(66, 66, 66);
  border: 10px solid rgb(0, 0, 0);
  color: rgb(255, 251, 0);
  font-family: 'Times New Roman', Times, serif;
  text-align: center;
  font-size: 19px;
  border-radius: 10px 10px 10px 10px;
  padding: 50px;
  display: flex;
  width: 30%;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;


}


</style>
