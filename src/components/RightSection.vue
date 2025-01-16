<template>
  <div class="greeting-text">Hi,</div>
  <div class="sub-greeting-text">Here's who i am and what i do</div>
  <div class="actions">
    <button class="btn primary">Resume</button>
    <button class="btn secondary">Projects</button>
  </div>
</template>

<style>
.greeting-text {
  font-size: 100px;
  line-height: 1.2em;
}

.sub-greeting-text {
  font-size: 25px;
}

.actions{
  display: flex;
  width: 100%;
  gap: 8px;
  padding: 16px 0;
}

.actions > .btn{
  border: none;
  border-radius: 4px;
  padding: 12px;
  width: 200px;
  text-transform: capitalize;
  cursor: pointer;
}

.actions > .btn:hover{
  background-color: #efeaea !important;
  border: 1px solid #ff926e !important;
  color: #ff926e !important;
}

.actions > .btn.primary{
  background-color: #ff926e;
  color: white;
}

.actions > .btn.secondary{
  background-color: #fcfcfc;
  border: 1px solid #ff926e;
  color: #ff926e;
}

</style>