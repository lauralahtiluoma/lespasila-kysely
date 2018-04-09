# lespasila-kysely

<form>
        <div id="lomake">
        
        </div>
        <button>Lähetä</button>
        </form>
      
        
     

      <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
        
          <script>
              var items=[];
        $.getJSON( "http://167.99.253.212:8080/lespasila/", function( data ) {
         $.each( data, function( key, d ) {
    items.push( d.kysymys + "<br> ");
    items.push("<input type=text id=" + d.id + "><br>")
});
 $( "<div/>", {
   "class": "my-new-list",
    html: items.join( "" )
    }).appendTo( "#lomake" );
});


        </script>
