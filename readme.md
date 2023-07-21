<h1 align="center"> Framework Jquery </h1>


<section>
<h2>Entendendo jquery</h2>
<div style="font-size:18px;">
 <p>Podemos iniciar o jquery com yarnn add -D jquery ou CDN referenciando no arquivo.js :</p>

<p> O $ referencia-se ao jquery ou </p>
<p>  utilize $()  onde ele pode receber funçoes e seletores $('div') onde ele vai selecionar as div</p>
</div>

<p style="font-size:18px;"> basic jquery 
</p>

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
<p style="font-size:18px;"> função:</p>

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
<div>

<p style="font-size:18px;"> Seletores :</p>


              // ...
        /*   seletor id */
        $('#feira') // # = pegando seletor id
        .addClass('destaque') // adicionar clase
        .removeClass('destaque') // ira remover a classe

        /* peganado seletor li */
        $('li')
        .addClass('destaque') 

        /* pegando atributo */
        $('[wm-obrigatorio]')
        .removeClass('destaque') 
        // vai remover class destaque do atributo
        
        /*  pegando a classe*/
        $('li.opcional')
        .removeClass('destaque')

        /* referenciando  */
        $('div p span').addClass('destaque')

        /*  Exclusivo do JQuery */
        //primeiro elemento li
        $('li:first') 
        .css('border','solid 2px yellow') //adiciona atributo css
        
        /*  oddd são os impares */
        $('li:odd')
        .css('border','solid 10px orange')

        /* gt(1) */
        $('li:gt(1)')
        css('border','solid 10px white')

        /* :not(:last)  ultimo */
        $('li:not(:last)').css('border','none')

        /* contains  utilizado para  ver se tem determinada letra */
        $('li:contains("r")').css('background-color','black')
</div>
<div>
<p style="font-size:18px;"> formulario </p>

            /* formulario: */

        $('form *') // formulario * seleciona tudo
        .hide() //escondido

        $('form :text') //:text e filtro
        $('form :password').show()
        $('form :checkbox').show()
        $('form :radio').show()
        $('form :file').show()

</div>
<div></div>
</section>