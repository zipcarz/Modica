Modica
======

1
2
3
4
5
6
7
8
9
$( ".container" )
  .contents()
    .filter(function() {
      return this.nodeType === 3;
    })
      .wrap( "<p></p>" )
      .end()
    .filter( "br" )
    .remove();
