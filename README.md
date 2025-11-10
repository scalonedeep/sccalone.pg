<html lang="es">
"Tus sueños",
"Cómo pensás en el futuro",
"Tu orgullo",
"Cómo la vivís en el liceo",
"Tu forma de seguir adelante",
"Que sos muy cómica",
"Tus imperfecciones",
"Te amo, no sé qué poner",
"Te gusta Anuel",
"Sos ree sociable",
"Cómo querés a la gente",
"Tu olor",
"Tu mirada (cuando me mirás)",
"Tus audios",
"Que sos ree única",
"Cómo no te importa lo que diga la gente",
"Cómo sos vos con todos flow, me explico?",
"Porque me das amor",
"Tenés tremendo pelo",
"Tu sonrisa",
"Cómo sos ree cariñosa mall",
"Cómo cuidás a tu hermano",
"Cómo te pones nerviosa por todo",
"Que seas ok",
"Tus mi vida",
"Cómo me decís amor",
"Cómo decís dea",
"Cómo pensás en el futuro",
"Tenés tremendos stikers",
"Que creés que me ganás en todo pero no",
"Cómo le llenas de amor todo"
];


let texto = document.getElementById('reason');
let boton = document.getElementById('nextBtn');
let usados = new Set();


function razonRandom(){
if(usados.size === razones.length){
usados.clear();
}
let i;
do{
i = Math.floor(Math.random() * razones.length);
}while(usados.has(i));
usados.add(i);
return razones[i];
}


boton.addEventListener('click', ()=>{
texto.textContent = razonRandom();
});
</script>
</body>
</html>
