<template>
  <div class="q-pa-md">
    <q-table title="Users" :rows="rows" :columns="columns" row-key="nome" />
  </div>
 </template>
 
 <script>
 import { defineComponent } from "vue";
 
 export default defineComponent({
  name: "UsersTemplate",
  data() {
    return {
      rows: [
        {
          nome: "Luiz Medeiros",
          email: "luiz@email.com",
          telefone: 999999999,
          funcao: "Programador",
        },
        {
          nome: "Rebeca Maria",
          email: "rebeca@email.com",
          telefone: 2222222222,
          funcao: "Web Designer",
        },
        {
          nome: "Lucas Santos",
          email: "lucas@email.com",
          telefone: 3333333333,
          funcao: "Programador Android",
        },
      ],
      columns: [
        {
          name: "nome",
          align: "left",
          label: "Nome",
          field: "nome",
          sortable: true,
        },
        {
          name: "email",
          align: "left",
          label: "E-mail",
          field: "email",
          sortable: true,
        },
        {
          name: "telefone",
          align: "left",
          label: "Telefone",
          field: "telefone",
          sortable: true,
        },
        {
          name: "funcao",
          align: "left",
          label: "Função",
          field: "funcao",
          sortable: true,
        },
      ],
    };
  },
 });
 </script>