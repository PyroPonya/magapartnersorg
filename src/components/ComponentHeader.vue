<template>
  <div class="header_container">
    <a href="">
      <div class="logo"></div>
    </a>
    <div class="controls">
      <a href="https://backoffice.megapartners.org/partner/login">
        <div class="btn login">login</div>
      </a>
      <a href="https://backoffice.megapartners.org/partner/register">
        <div class="btn signup">sing&nbsp;up</div>
      </a>
      <div class="select language_selector">•&nbsp;EN</div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    return {};
  },
};
</script>

<style scoped>
.header_container {
  width: 100%;
  border-bottom: 1px solid #282841;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  padding-bottom: 2rem;
  margin-bottom: 2rem;
}
.logo {
  background-image: url(./icons/megapartners_logo.svg);
  width: 470px;
  height: 28px;
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
}
.controls {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
.btn {
  width: 118px;
  height: 50px;
  background: #ffffff;
  border: 1px solid #282841;
  border-right: 0;
  font-weight: 500;
  font-size: 16px;
  line-height: 20px;
  color: #131326;
  display: flex;
  align-items: center;
  justify-content: center;
  text-transform: uppercase;
}
.select {
  width: 77px;
  height: 50px;
  background: none;
  border: 1px solid #282841;
  font-weight: 500;
  font-size: 16px;
  line-height: 20px;
  color: #131326;
  display: flex;
  align-items: center;
  justify-content: center;
  text-transform: uppercase;
}
.btn:hover,
.select:hover {
  background: #4790fe;
  color: #ffffff;
  cursor: pointer;
}
</style>
