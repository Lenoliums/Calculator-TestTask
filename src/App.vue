<template>
  <div id="calculator-conteiner" class="flex-center">
    <div id="calculator">

      <div id="buttons-conteiner" class="flex-center">
        <div class="button flex-center" v-for="button in buttons">
          <div class="circl">{{button.symbol}}</div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return { 
        buttons:[
          {
            symbol: 'C',
            onClick: '',
          },
          {
            symbol: '√',
            onClick: '',
          },
          {
            symbol: '%',
            onClick: '',
          },
          {
            symbol: '/',
            onClick: '',
          },
          {
            symbol: '7',
            onClick: '',
          },
          {
            symbol: '8',
            onClick: '',
          },
          {
            symbol: '9',
            onClick: '',
          },
          {
            symbol: '×',
            onClick: '',
          },
          {
            symbol: '4',
            onClick: '',
          },
          {
            symbol: '5',
            onClick: '',
          },
          {
            symbol: '6',
            onClick: '',
          },
          {
            symbol: '-',
            onClick: '',
          },
          {
            symbol: '1',
            onClick: '',
          },
          {
            symbol: '2',
            onClick: '',
          },
          {
            symbol: '3',
            onClick: '',
          },
          {
            symbol: '+',
            onClick: '',
          },
          {
            symbol: '00',
            onClick: '',
          },
          {
            symbol: '0',
            onClick: '',
          },
          {
            symbol: ',',
            onClick: '',
          },
          {
            symbol: '=',
            onClick: '',
          }
        ],
        result: '',
        culculations: ''
      };
    }
  }
</script>


<style>
*{
  box-sizing: border-box;
}
body{
  margin: 0;
  height: 100vh;
  background: linear-gradient(122.76deg, #FFA2A2 4.09%, #FF7B7B 91.04%);
}
  #app{
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  #calculator{
    width: 100%;
    height: 100%;
    border-radius: 18px;
    background: linear-gradient(155.23deg, #28518E 0%, #3A77D1 100%);
    box-shadow: 0px 82px 158px 0px #00000059;
    padding: 47px;
  }
  #calculator-conteiner{
    max-width: 616px;
    max-height: 876px;
    height: 92vh;
    width: 64.7vh;
    margin: auto;
    border-radius: 18px;
    background: rgba(255, 255, 255, 0.2);
    padding: 38px 31px
  }
  .flex-center{
    display: flex;
    align-items: center;
    justify-content: center;
  }
  @media only screen and (max-width: 768px) {
  /* For mobile phones: */
  #calculator-conteiner{
    max-width: unset;
    max-height: unset;
    width: 100vw;
    height: 100lvh;
    border-radius: 0;
  }

}
.button{
  
    flex-basis: 23%;
    height: 19%;
    
  }
  #buttons-conteiner{
    position: relative;
    bottom: 0;
    width: 100%;
    height: 60%;
    flex-wrap: wrap;
    gap:5px
  }
  .circl{
    color: white;
    text-align: center;
    border-radius: 100%;
    aspect-ratio: 1 / 1;
    height: 100%;
    display: table-cell;
    vertical-align: middle;
  }
  .circl:hover{
    background-color: rgba(255, 255, 255, 0.12);
  }
</style>
