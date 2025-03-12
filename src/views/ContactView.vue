<template>
  <section>
    <div class="heading">Contact</div>
    <div class="col">
      <div class="row">
        <div class="text">
          Your Name
        </div>
        <input type="text" class="input-text"/>
      </div>
      <div class="row">
        <div class="text">
          Message
        </div>
        <textarea type="text" rows="5" class="input-text"/>
      </div>
    </div>
  </section>

</template>

<style>

section .col {
  display: flex;
  width: 100%;
  flex-direction: column;
  align-items: center;
}

section .col .row {
  display: flex;
  justify-content: space-between;
  width: 600px;
  padding: 10px;
  border: 2px solid #ff926e;
  background-color: white;
  border-radius: 4px;
  margin: 12px 0;
  transition: border-color 0.5s;
}

section .col .row:hover{
  border-color: #d53307;
}

section .col > .row > .text {
  color: black;
  font-size: 18px;
  font-weight: 600;
  margin: 0 10px;
  width: 150px;
}

section .col > .row > .input-text {
  border: 1px solid #efeaea;
  width: 100%;
  outline: none;
  border-radius: 4px;
  padding: 4px;
  font-size: 18px;
  color: #ff926e;
  transition: border-color 0.5s;
}

section .col > .row > .input-text:hover{
  border-color: #ff926e;
}

section .heading {
  color: #dad7d3;
  font-size: 32px;
  padding: 12px;
  font-weight: bolder;
  line-height: 1.5rem;
  border-bottom: #eb4813 2px solid;
}


</style>