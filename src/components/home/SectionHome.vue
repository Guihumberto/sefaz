<template>
  <section>
    <div class="container">
      <h2 class="spaceh2">Serviços</h2>
      <div class="even-columns">
        <div class="box" v-for="item, i in services" :key="i">
          <p class="text-center">
            {{ item }}
          </p>
        </div>
      </div>
      <div class="btnWrapper">
        <v-btn variant="outlined" color="primary" width="300px">Mais Serviços</v-btn>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    data(){
      return{
        services:['DARE', 'IPVA', 'SEFAZ.NET', 'ITCD',  'ISENÇÕES IPVA E ICMS/DESONERAÇÕES', 'DOWNLOAD XML(NF-E)/DOC. FISCAIS ELETRÔNICOS', 'CERTIDÕES', 'LEGISLAÇÃO', 'CADASTRO/ATIVAÇÃO', 'NOTA FISCAL AVULSA ELETRÔNICA (NFA-E)', 'LEGISLAÇÃO', 'CADASTRO/ATIVAÇÃO']
      }
    }
  }
</script>

<style lang="scss" scoped>
.container{
  display: flex;
  flex-direction: column;

}
.even-columns{
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
  gap: 5px;
  width: 100%;
}
.box{
  width: 14rem;
  height: 5rem;
  background-color: var(--primary-color);
  color: white;
  font-weight: 600;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 1rem;
  transition: .5s ease;
}
.box:hover{
  transform: scaleX(1.1);
}
.btnWrapper{
  display: flex;
  justify-content: center;
  padding: 2rem;
}

</style>
