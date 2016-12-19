var remOnClick = function() {
    this.remove();
}
var changeHeader = function( ) {
    var h = document.getElementById('h');
    h.innerHTML = this.innerHTML;    
}

var resetHeader = function() {
    var h = document.getElementById('h');
    h.innerHTML = "Hello World!";
}

var b = document.getElementById( 'b' );
b.addEventListener('click',
                   function() {
                       var elem = document.createElement('li');
                       var text = document.createTextNode("New Thing!");
                       elem.appendChild(text);
                       elem.addEventListener('click', remOnClick );
                       elem.addEventListener('mouseover', changeHeader);
                       elem.addEventListener('mouseout', resetHeader);
                       var list = document.getElementById('thelist');
                       list.appendChild(elem);
                   });

var l = document.getElementById('thelist').childNodes;
for( var i = 0; i< l.length; i++ ){
    l[i].addEventListener('click', remOnClick);
    l[i].addEventListener('mouseover', changeHeader);
    l[i].addEventListener('mouseout', resetHeader);
}

var b2 = document.getElementById('b2');
b2.addEventListener('click',
                    function() {
                        var list = document.getElementById('fiblist');
                        var elem = document.createElement('li');
                        if( list.childNodes.length < 3 ){
                            elem.innerHTML = 1;
                        }else{
                            elem.innerHTML = parseInt(list.childNodes[list.childNodes.length-1].innerHTML) + parseInt(list.childNodes[list.childNodes.length-2].innerHTML );
                        }
                        list.appendChild( elem );
                    });



    
