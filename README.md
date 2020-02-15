
console.log("Bienvenido a seguros TK-U.")
var nombreCompleto = prompt("Por favor ingrese el nombre completo:", "Nombres y apellidos");
console.log("Muchas Gracias" + nombreCompleto);
var diaNacimiento = prompt("Ingrese el día de nacimiento", "Ejemplo: Si nació el 22 de enero, solamente ingresar 22");
var mesNacimiento = prompt("Ingrese el mes de nacimiento", "Ejemplo: Si nació en enero, solamente ingresar 1 porque es el mes 1");
var anioNacimiento = prompt("Ingrese el año de nacimiento", "Ejemplo: Si nació el 22 de enero de 1987, solamente ingresar 1987");

var conyuge = prompt("¿Tiene cónyuge?", "SI/NO");
var hijos = prompt("¿Tiene hijos?", "SI/NO");
var cantidadHijos = prompt("Ingrese la cantidad de hijos menores de 21 años:", "Por favor ingrese únicamente números");
    
var edad = 34;
var edadconyuge = 34;
   

const precioBase = 250;

const comision = precioBase * 0.30;



if (edad<18){
  alert("No se le puede asegurar");
}else if (edad>=20, edad<21){
  alert("No se le aplica recargos");
}else if (edad>=21, edad<26){
  console.log("Recargos por edad:Q"+precioBase * 0.01);
}else if (edad>=26, edad<31){
  console.log("Recargos por edad:Q"+precioBase * 0.02);
}else if (edad>=31, edad<41){
  console.log("Recargos por edad:Q"+precioBase * 0.05);
}else if (edad>=41, edad<51){
  console.log("Recargos por edad:Q"+precioBase * 0.08);
}else if(edad>=51, edad<65){
  console.log("Recargos por edad:Q"+precioBase * 0.12);
}else {
  alert("es mayor de 65 años");
}

if (conyuge  == "SI", edadconyuge<30){
  console.log("Recargos por conyuge:Q"+precioBase * 0.01);
}else if (edadconyuge>=30, edadconyuge<40){
  console.log("Recargos por conyuge:Q"+precioBase * 0.02);
}else if (edadconyuge>=40, edadconyuge<50){
  console.log("Recargos por conyuge:Q"+precioBase * 0.03);
}else if (edadconyuge>=50, edadconyuge<70){
  console.log("Recargos por conyuge:Q"+precioBase * 0.05);
}

if (hijos == "SI"){
  console.log("Recargos por hijos:Q"+precioBase * 0.01 * cantidadHijos);
}

console.log("totalPagar="+precioBase + comision);
