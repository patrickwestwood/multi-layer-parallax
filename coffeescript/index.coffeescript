# Tutorial: https://medium.com/@PatrykZabielski/how-to-make-multi-layered-parallax-illustration-with-css-javascript-2b56883c3f27

window.addEventListener 'scroll', (event) ->
  topDistance = @pageYOffset 
  layers = document.querySelectorAll("[data-type='parallax']")
  
  for layer in layers
    depth = layer.getAttribute('data-depth')
    movement = -(topDistance * depth)
    translate3d = 'translate3d(0, ' + movement + 'px, 0)'
    layer.style['-webkit-transform'] = translate3d
    layer.style['-moz-transform'] = translate3d
    layer.style['-ms-transform'] = translate3d
    layer.style['-o-transform'] = translate3d
    layer.style.transform = translate3d
  return