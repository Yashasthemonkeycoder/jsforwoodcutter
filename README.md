<script>
      // long code, sorry

alert("welcome to the game The Woodcutter!")
alert("The goal of this game is to sell and make the wood properly to get 100K credits")
alert("INSTRUCTIONS:- 1.Clicking on the tree provides you one wood.    2.using powerups you can get 2x,3x and 4x wood.     3. dealing with a bussiness man provides you 2x credits at once.       4. getting 2x wood will provide you 2x wood at once")
alert("Tap the tree to start the game")
alert("Thats it. Play fair - yashas the monkey coder")
alert("hi lohith!")
var wood1 = 0;
var crefits = 0;
var wood3 = 0;
var wood4 = 0;
var woodd = 0;
var dous = 0;
var sus = 0;
var make = 0;

function wood(){
    wood1+=1;
    document.getElementById("cou").innerHTML="wood:"+wood1
    document.getElementById("sell").innerHTML="Sell  wood for "+wood1/2+" $"
    document.getElementById("wor").innerHTML=""
    document.getElementById("music").play()
    if(dous==1){
        wood1+=1
        document.getElementById("cou").innerHTML="wood:"+wood1
    }
    if(dous==2){
        wood1+=2
        document.getElementById("cou").innerHTML="wood:"+wood1
    }
    if(dous==3){
        wood1+=3
        document.getElementById("cou").innerHTML="wood:"+wood1
        
    }
}    
function pay(){
    crefits+=wood1/2;
    wood3 += wood1/2; document.getElementById("cre").innerHTML="Credits: "+crefits
    wood1-=wood1;
    document.getElementById("cou").innerHTML="wood:"+wood1
    if(crefits > 0){
        var al = alert(crefits+" current balance ✓");
        document.getElementById("sell").innerHTML="Sell  wood for "+wood1/2+" $"
    }
    else{
        alert("please gain some money by cutting trees.. payment cancelled ×")
    }
    if(crefits >= 100000){
       var crefits2 = crefits/1000+'K'
       document.getElementById("cre").innerHTML="Credits: "+crefits2
    }
    if(crefits>=100000){
    alert("working...")
    document.getElementById("cou").style.display="none"
    document.getElementById("cre").style.display="none"
    document.getElementById("wor").style.display="none"
    document.getElementById("butttt").style.display="none"
    document.getElementById("imag").style.display="none"
    document.getElementById("sell").style.display="none"
    document.getElementById("bat").style.display="none"
    document.getElementById("bat1").style.display="none"
    document.getElementById("bat2").style.display="none"
    document.getElementById("bat3").style.display="none"
    document.getElementById("anime").style.display="true"
    document.getElementById("anime").style.display="true"
    document.getElementById("conti").style.visibility="visible"
    document.getElementById("foot1").style.visibility="hidden"
    document.getElementById("foot2").style.display="none"
    document.getElementById("butt9").style.visibility="hidden"
    
}
    

}
function worker(){
    if(crefits >= 200){
        if(wood1>0){
            crefits-=200;
         document.getElementById("cre").innerHTML="Credits: "+crefits
         wood1 = wood1+wood1;
         document.getElementById("cou").innerHTML="wood:"+wood1
         document.getElementById("butttt").style.display="none"
         alert("you have multiplied "+wood1/2+" wood to "+wood1+" wood")
        }
        else{
            alert("you must have more than one wood to multiply ×")
        }
    }
    else{
        alert("you need to have 200$, payment cancelled ×");
    }
}
function deal(){
    if(wood1>=1000){
        crefits+=wood1;
        alert("you have dealed "+wood1+" with the bussiness man and he has gave you "+wood1+" credits")
        document.getElementById("cre").innerHTML="Credits: "+crefits
         wood1-=wood1;
         document.getElementById("cou").innerHTML="wood:"+wood1
         document.getElementById("sell").innerHTML="Sell  wood for "+wood1/2+" $"
         document.getElementById("bat").style.display="none"
    }
    else{
        alert("you need to have atleast 1000 wood to sell the bussiness man");
    }
}
function deal1(){
     if(crefits>=500){
         dous+=1
         crefits-=500
         alert("you have got 2x wood");
         sus+=1
         document.getElementById("cre").innerHTML="Credits:"+crefits
         document.getElementById("bat1").style.display="none"
         
     }
     
     else{
         alert("you need to have 500$ to get 2x wood");
}
}
function deal2(){
    if(crefits>=700){
        if(sus==1){
            dous+=1
            crefits-=700
            sus+=1
            alert("you have got 3x wood")
            document.getElementById("cre").innerHTML="Credits:"+crefits
            document.getElementById("bat2").style.display="none"
            
        }
        else{
            alert("you need to unlock 2x first")
        }
        
    }
    else{
        alert("you need to have 700$ to get 3x wood");
    }
}
function deal3(){
    if(crefits>=1500){
        if(sus==2){
            dous+=1
            crefits-=1500
            alert("you have got 4x wood")
            document.getElementById("cre").innerHTML="Credits:"+crefits
            document.getElementById("bat3").style.display="none"
            document.getElementById("butt9").style.visibility="hidden"
        }
        else{
            alert("you need to unlock 3x wood first")}
        if(sus==1){
            alert("you need to unlock 2x and 3x wood first")
        }
        
        
    }
    else(
        alert("you need to have 1500$ to unlock 4x wood")
    )
}
function counti(){
    document.getElementById("anime").style.display="true"
    document.getElementById("anime").style.visibility="visible"
    document.getElementById("conti").style.visibility="hidden"
}
function okbe(){
    alert("working...")
    document.getElementById("anime").style.display="none"
    document.getElementById("anime").style.visibility="hidden"
    document.getElementById("conti").style.visibility="hidden"
    document.getElementById("latpa").style.visibility="visible"
    

}



</script>
