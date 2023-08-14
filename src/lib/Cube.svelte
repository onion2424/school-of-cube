<script lang="ts">
  let faces = ['left', 'right', 'top', 'bottom', 'back', 'front'];
  let number = [...Array(26)]

  let colors = ['blue', 'green', 'white', 'yellow', 'orange', 'red'];
	let pieces = document.getElementsByClassName('piece') as HTMLCollectionOf<HTMLElement>;

// Returns j-th adjacent face of i-th face
function mx(i, j) {
	return ([2, 4, 3, 5][j % 4 |0] + i % 2 * ((j|0) % 4 * 2 + 3) + 2 * (i / 2 |0)) % 6;
}

function getAxis(face) {
	return String.fromCharCode('X'.charCodeAt(0) + face / 2); // X, Y or Z
}

// Moves each of 26 pieces to their places, assigns IDs and attaches stickers
function assembleCube() {
	function moveto(face) {
		id = id + (1 << face);
    var elm = document.createElement('div');
		pieces[i].children[face].appendChild(elm)
			.setAttribute('class', 'sticker ' + colors[face]);
		return 'translate' + getAxis(face) + '(' + (face % 2 * 4 - 2) + 'em)';
	}
	for (var id, x, i = 0; id = 0, i < 26; i++) {
		x = mx(i, i % 18);
		pieces[i].style.transform = 'rotateX(0deg)' + moveto(i % 6) +
			(i > 5 ? moveto(x) + (i > 17 ? moveto(mx(x, x + 2)) : '') : '');
		pieces[i].setAttribute('id', 'piece' + id);
	}
}

function getPieceBy(face, index, corner) {
	return document.getElementById('piece' +
		((1 << face) + (1 << mx(face, index)) + (1 << mx(face, index + 1)) * corner));
}



document.ondragstart = function() { return false; }
window.addEventListener('load', assembleCube);
//scene.addEventListener('mousedown', mousedown);
</script>
<div class="scene" >
	<div class = "pivot centered" style = 'transform: rotateX(0deg) rotateY(0deg)'>
    <div class ="cube">
      {#each number as num}
      <div class="piece">
        {#each faces as face}
        <div class="element {face}"/>
        {/each}
      </div>
      {/each}
    </div>
  </div>
</div>
<style lang="scss">

  $base-color: #0A0A0A;
  $ground-color: #2F2F31;
  $element-size: 2em;
  $sticker-size: 95%;
  $rounded: 10%;
  $cube-scale: 1;
  $faces: (left: (0, -90, 180), right: (0, 90, 90), back: (0, 180, -90), front: (0, 0, 0), bottom: (-90, 0, -90), top: (90, 0, 180));
  $colors: (blue: #001ca8, green: #006E16, white: #DDD, yellow: #E0AE00, orange: #FF5000, red: #DF0500);
  
  .text {
    text-align: center;
    font: { family: Helvetica; size: .8rem; }
    color: grey;
    pointer-events: none;
  }
  
  .centered {
    position: absolute;
    top: 0; bottom: 0; left: 0; right: 0;
    margin: auto;
  }
  
  .scene {
    width: 100%;
    height: 100%;
    perspective: 1200px;
    transform-style: preserve-3d;
    > .pivot {
      width: 0;
      height: 0;
      transition: .18s;
    }
    .anchor {
      width: $element-size;
      height: calc($element-size * 3);
    }
    div {
      position: absolute;
      transform-style: inherit;
    }
  }
  
  #piece4 > .element.top > .sticker {
    background-image: URL('http://i63.tinypic.com/25hh1xu.png');
    background-size: cover;
  }
  
  .cube {
    font-size: calc($cube-scale * 100%);
    margin-left: calc((-1 * $element-size) / 2);
    margin-top: calc((-1 * $element-size) / 2);
  
    > .piece {
      width: calc($element-size - .1em);
      height: calc($element-size - .1em);
      > .element {
        width: 100%;
        height: 100%;
        background: $base-color;
        outline: 1px solid transparent; // firefox aliasing
        border: .05em solid $base-color { radius: $rounded }
        @each $face, $angles in $faces {
            &.#{$face} {
              transform: rotateX + '(' + nth($angles, 1) + 'deg)'
                         rotateY + '(' + nth($angles, 2) + 'deg)'
                         rotateZ + '(' + nth($angles, 3) + 'deg)' translateZ(calc($element-size / 2));
            }
        }
        > :global(.sticker) {
          @extend .centered;
          transform: translateZ(2px);
          width: $sticker-size;
          height: $sticker-size;
          border-radius: $rounded;
          outline: 1px solid transparent; // firefox aliasing
          box-shadow: inset .05em .05em .2rem 0 rgba(white, .25),
                      inset -.05em -.05em .2rem 0 rgba(black, .25);
        }
      }
    }
  
  }
</style>