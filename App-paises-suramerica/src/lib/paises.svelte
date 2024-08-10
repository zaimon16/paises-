<script>
    export let pais;
    let p;
    /*[0]=nombre_pais [1]=capital [2]=Población [3]=moneda [4]=area [5]=bandera*/
    const paises = {
        colombia: [
            "Colombia",
            "Bogota",
            "51,2 millones",
            "pesos colombianos",
            "1,142 millones km2",
            "colombia.jpg",
        ],
        venezuela: [
            "Venezuela",
            "Caracas",
            "28,2 millones",
            "bolivar",
            "916.445 km2",
            "venezuela.jpg",
        ],
        ecuador: [
            "Ecuador",
            "Quito",
            "17,8 millones",
            "dolar estadunidense",
            "256.370 km2",
            "ecuador.jpg",
        ],
        peru: [
            "Peru",
            "Lima",
            "33,72 millones",
            "sol peruano",
            "1.285.215 km2",
            "peru.jpg",
        ],
        brasil: [
            "Brasil",
            "Brasilia",
            "214,3 millones",
            "real brasileño",
            "8,51 km2",
            "brasil.jpg",
        ],
        paraguay: [
            "Paraguay",
            "Asuncion",
            "6.109.644 millones",
            "guarani",
            "15,02 km2",
            "paraguay.jpg",
        ],
        bolivia: [
            "Bolivia",
            "Sucre",
            "12.186.073 millones",
            "boliviano",
            "11,09 km2",
            "bolivia.jpg",
        ],
        uruguay: [
            "Uruguay",
            "Montevideo",
            "3,444,263 millones",
            "uruguayan peso",
            "19.5 km2",
            "uruguay.jpg",
        ],
        argentina: [
            "argentina",
            "buenos aires",
            "4,444,263 millones",
            "peso argentino",
            "2.78 km2",
            "Argentina.jpg",
        ],
        chile: [
            "chile",
            "santiago",
            "2,423,263 millones",
            "peso chileno",
            "756.626 km2",
            "chile.jpg",
        ],
    };
    p = paises[pais];
</script>

<div class="main">
    <div class="col1">
        <img
            src="./src/assets/{p[5]}"
            alt="Bandera_Colombia"
            width="300"
            height="200"
        />
    </div>
    <div class="col2">
        <div class="linea"><strong>Pais:</strong>{p[0]}</div>
        <div class="linea"><strong>capital:</strong>{p[1]}</div>
        <div class="linea"><strong>poblacion:</strong>{p[2]}</div>
        <div class="linea"><strong>moneda:</strong>{p[3]}</div>
        <div class="linea"><strong>Extension:</strong>{p[4]}</div>
    </div>
</div>

<style>
    .main {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-gap: 5px;
        grid-auto-rows: minmax(100px, auto);
        border-radius: 10px;
        border-style: solid;
        border-color: rgb(0, 0, 0);
        border-width: 2px;
        margin: left;
        width: 600px;
        box-shadow: 5px 5px 5px black;
        margin-right: 5px;
        margin-bottom: 10px;
    }
    .col1 {
        grid-column: 1;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
    }
    .col2 {
        grid-column: 2;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
        border-color: black;
        width: max-content;
    }
    strong {
        color: rgb(0, 0, 0);
        font-weight: bolder;
    }
    .linea {
        font-size: 20px;
        margin-bottom: 18px;
    }
</style>
