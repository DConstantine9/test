<template>
  <div class="home">
    <div class="block">
      Write a new task
    </div>
    <div class="block2">
      <label>
        <input type="checkbox" class="checkbox">
        <span class="checkbox-custom"></span>
      </label>
      <input type="text" placeholder="Write a new task">
      <i class="far fa-calendar" id="calendar"></i>
      <select name="" id="">
        <option value="No List">No List</option>
        <option value="List 1">List 1</option>
      </select>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
}
</script>

<style scoped>

.block {
  color: #5C5F66;
  height: 40px;
  width: 400px;
  border-radius: 12px;
  text-align: left;
  vertical-align: middle;
  padding: 10px;
  box-sizing: border-box;
  background:#CFD1DB;
  margin-bottom: 10px;
}

.block:hover {
  background: #C7C9D3;
  cursor: pointer;
}

.block2 {
  height: 40px;
  width: 400px;
  border-radius: 12px;
  text-align: left;
  vertical-align: middle;
  padding: 10px;
  box-sizing: border-box;
  box-shadow: 0 14px 35px rgba(87, 87, 87, 0.25);
  background: white;
}

input[type="text"] {
  border: none;
  outline: none;
}

.checkbox {
  display: none;
}

.checkbox-custom {
  display: inline-block;
  position: relative;
  cursor: pointer;
  width: 20px;
  height: 20px;
  background: #EAE8EA;
  border-radius: 5px;
}

.checkbox:checked + .checkbox-custom::before {
  content: "";
  display: block;
  position: absolute;
  background: rgb(49, 218, 49);
  top: 0px;
	right: 0px;
	bottom: 0px;
	left: 0px;
  border-radius: 5px;
}

#calendar {
  border-radius: 7px;
  background: #F2F3F6;
  padding: 7px 9px;
}

select {
  border: none;
  outline: none;
  border-radius: 7px;
  background: #F2F3F6;
  padding: 7px 9px;
}

select option {
  padding: 10px;
}

</style>