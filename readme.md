<h1 align="center"> Framework Jquery </h1>


<section>
<h2>Entendendo jquery</h2>
<div style="font-size:18px;">
 <p>Podemos iniciar o jquery com yarnn add -D jquery ou CDN referenciando no arquivo.js :</p>

<p> O $ referencia-se ao jquery ou </p>
<p>  utilize $()  onde ele pode receber funçoes e seletores $('div') onde ele vai selecionar as div</p>
</div>

<div>
   // ...

     
        $('div')
        .hide(500)  // funcao esconde
        .show(5000)  // função mostrar
        .fadeOut(5000)   // Oculte os elementos correspondentes tornando-os transparentes.
        console.log(
            $('div')
    // ele vai me da de fato elemento dom q esta 
    // assosiado ao seletor
            .get(0) 
        )
        console.log(
            $.isEmptyObject({
               // aqui a gente passs obj p/ verificar 
            })
            )

            console.log(
                $ 
                .inArray(3,// verifico um determinado numero de array
                [1,2,3]
                ))
</div>
<div>
<p> Jquery Css</p>

       // criando uma funcao p/ mudar fundo do body
        ========== funcao ==================
            $.fn.fundoVerde = function (){
                
                //colocar propriedade css
                this.css(
                    // propriedade e valor 
                    'background-color','green'
                    // igual background-color:green
                    )
                    // pra encadear eu faço retorno:
                    return this
                }
                    
                  ======= /*  aplicando: */ =============
                $('body') // seleciono elemento
                .fundoVerde() // passo função
                .hide(1000)

</div>
<div></div>
<div></div>
<div></div>
</section>