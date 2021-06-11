<template>
  <div class="register">
    <h1>{{ msg }}</h1>
    Employee Name:<input
      type="text"
      class="hlo"
      name="username"
      id="name"
    /><br /><br />
    Role&emsp;&emsp;&nbsp;&nbsp;&nbsp;:
    <select id="role" name="role" class="hlo">
      <option class="hlo" value="Software Designer">Developer</option>
      <option class="hlo" value="QA">QA</option>
      <option class="hlo" value="Fullstack Developer">FSD Developer</option>
      <option class="hlo" value="Analyst">Product Designer</option>
    </select>
    <br /><br />
    Leads&emsp;&emsp;&nbsp;:
    <select id="leads" name="leads" class="hlo" minlength="3" maxlength="15">
      <option class="hlo" value="Intern">Intern</option>
      <option class="hlo" value="Employee">Employee</option>
    </select>
    <br /><br />

    <input type="submit" value="SAVE" id="sub" /><br /><br /><br />
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.register {
  margin: auto;
  width: 100%;
  background: rgba(0, 0, 0, 0.1);
  border: 2px solid white;
  padding: 10px;
}
.hlo {
  width: 40%;
  padding: 8px;
  border-radius: 10px;
  font-size: 18px;
  font-family: serif;
  background: rgb(154, 158, 157);
}
#sub {
  width: 150px;
  padding: 5px;
  text-align: center;
  font-family: serif;
  font-size: 18px;
}
</style>
