<script lang="ts">
    let face = ["none", "blue", "orange", "white", "red", "yellow", "green"];
    export let classes = [
        "horizon location0 size3 arrow2",
        "vertical location0 size3 arrow1",
        "upper location6 size3 arrow1",
        "upper location3 size2 arrow2",
        "lower location3 size2 arrow1",
        "vertical location1 size3 arrow2"
    ];
    export let colors = new Array<number>(27);
    colors = [
        6, 6, 6, 
        6, 6, 6, 
        6, 6, 6,

        2, 2, 2, 
        3, 3, 3, 
        4, 4, 4,
        5, 5, 5, 
    ];
</script>

<div class="face">
    <div class="scene s-r6LgU90Jc_vZ">
        <div
            class="pivot centered s-r6LgU90Jc_vZ"
            style="transform: rotateX(0deg) rotateY(0deg);"
        >
            <div class="cube">
                {#each classes as elm}
                    <div class={elm} >
                        <span />
                    </div>
                {/each}
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateY(-2em) translateZ(2em) translateX(-2em);"
                >
                    <div class="element left s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[20]]}" />
                    </div>
                    <div class="element top s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[9]]}" />
                    </div>
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[0]]}">
                        </div>
                    </div>
                </div>
                <div
                    class="piece s-r6LgU90Jc_vZ"
                    style="transform: rotateX(0deg) translateY(-2em) translateZ(2em);"
                >
                    <div class="element top s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[10]]}" />
                    </div>
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[1]]}">
                        </div>
                    </div>
                </div>
                <div
                    class="piece s-r6LgU90Jc_vZ"
                    style="transform: rotateX(0deg) translateZ(2em) translateX(2em) translateY(-2em);"
                >
                    <div class="element right s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[12]]}" />
                    </div>
                    <div class="element top s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[11]]}" />
                    </div>
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[2]]}" >
                        </div>
                    </div>
                </div>
                
                <div
                    class="piece s-r6LgU90Jc_vZ"
                    style="transform: rotateX(0deg) translateZ(2em) translateX(-2em);"
                >
                    <div class="element left s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[19]]}" />
                    </div>
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[3]]}">
                        </div>
                    </div>
                </div>
                
                <div
                    class="piece s-r6LgU90Jc_vZ"
                    style="transform: rotateX(0deg) translateZ(2em);"
                >
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[4]]}">
                        </div>
                    </div>
                </div>

                <div
                    class="piece s-r6LgU90Jc_vZ"
                    style="transform: rotateX(0deg) translateZ(2em) translateX(2em);"
                >
                    <div class="element right s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[13]]}" />
                    </div>
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[5]]}">
                        </div>
                    </div>
                </div>

                <div
                    class="piece s-r6LgU90Jc_vZ"
                    style="transform: rotateX(0deg) translateX(-2em) translateY(2em) translateZ(2em);"
                >
                    <div class="element left s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[18]]}" />
                    </div>
                    <div class="element bottom s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[17]]}" />
                    </div>
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[6]]}">
                        </div>
                    </div>
                </div>
                <div
                    class="piece s-r6LgU90Jc_vZ"
                    style="transform: rotateX(0deg) translateY(2em) translateZ(2em);"
                >
                    <div class="element bottom s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[16]]}" />
                    </div>
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[7]]}">
                        </div>
                    </div>
                </div>
                <div
                    class="piece s-r6LgU90Jc_vZ"
                    style="transform: rotateX(0deg) translateX(2em) translateY(2em) translateZ(2em);"
                >
                    <div class="element right s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[14]]}" />
                    </div>
                    <div class="element bottom s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[15]]}" />
                    </div>
                    <div class="element front s-r6LgU90Jc_vZ">
                        <div class="sticker {face[colors[8]]}">
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
</div>

<!--<Cube>-->
<style lang="scss">
    $base-color: #0a0a0a;
    $ground-color: #2f2f31;
    $element-size: 2em;
    $sticker-size: 95%;
    $rounded: 5%;
    $faces: (
        left: (
            0,
            -90,
            180,
        ),
        right: (
            0,
            90,
            90,
        ),
        back: (
            0,
            180,
            -90,
        ),
        front: (
            0,
            0,
            0,
        ),
        bottom: (
            -90,
            0,
            -90,
        ),
        top: (
            90,
            0,
            180,
        ),
    );
    $colors: (
        blue: #001ca8,
        green: #006e16,
        white: #ddd,
        yellow: #e0ae00,
        orange: #ff5000,
        red: #df0500,
    );

    :root {
        --cube-scale: 0.5;
    }

    .face {
        height: calc(170px * var(--cube-scale));
        width: calc(170px * var(--cube-scale));
    }

    .text {
        text-align: center;
        font: {
            family: Helvetica;
            size: 0.8rem;
        }
        color: grey;
        pointer-events: none;
    }

    .centered {
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
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
            transition: 0.18s;
        }
        .anchor {
            width: $element-size;
            height: calc($element-size * 3);
        }
        div {
            position: absolute;
            //transform-style: inherit;
        }
    }

    .cube {
        font-size: calc(var(--cube-scale) * 100%);
        margin-left: calc((-1 * $element-size) / 2);
        margin-top: calc((-1 * $element-size) / 2);
        > .piece {
            width: calc($element-size - 0.1em);
            height: calc($element-size - 0.1em);
            > .element {
                width: 100%;
                height: 100%;
                background: $base-color;
                outline: 1px solid transparent; // firefox aliasing
                border: 0.1em solid $base-color {
                    radius: $rounded;
                }
                &.front {
                    transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
                }
                &.top {
                    transform: rotateX(80deg) rotateY(0deg) rotateZ(0deg)
                        translateZ(1.5em);
                }
                &.bottom {
                    transform: rotateX(-80deg) rotateY(0deg) rotateZ(0deg)
                        translateZ(1.5em);
                }
                &.right {
                    transform: rotateX(0deg) rotateY(80deg) rotateZ(0deg)
                        translateZ(1.5em);
                }
                &.left {
                    transform: rotateX(0deg) rotateY(-80deg) rotateZ(0deg)
                        translateZ(1.5em);
                }
                > :global(.sticker) {
                    @extend .centered;
                    transform: translateZ(calc(8px * var(--cube-scale)));
                    width: $sticker-size;
                    height: $sticker-size;
                    border-radius: $rounded;
                    position: relative;
                    outline: 1px solid transparent; // firefox aliasing
                    box-shadow: inset 0.05em 0.05em 0.2rem 0 rgba(white, 0.25),
                        inset -0.05em -0.05em 0.2rem 0 rgba(black, 0.25);
                    &.none
                    {
                        display: none;
                    }
                }
            }
        }

        $sizes:(
        size1: 1,
        size2: 2,
        size3: 3
        );
        $locations:(
            location0: (-2em, -2em),
            location1: (0em, -2em),
            location2: (2em, -2em),
            location3: (-2em, 0em),
            location4: (0em, 0em),
            location5: (2em, 0em),
            location6: (-2em, 2em),
            location7: (0em, 2em),
            location8: (2em, 2em)
        );
        $arrow-size: 0.5em;
        $arrow-color : black;
        > div:not(.piece)
        {
            //background-color: rgba(255, 238, 0, 0.89);
            position: absolute;

            margin-top: 0px;
            // iosで必要だった
            z-index: 100;
            transform: translateZ(50px);
            @each $location, $index in $locations 
                {
                    &.#{$location}
                    {
                        left:nth($index, 1);
                        top:nth($index, 2);
                    }
                }
            &.arrow1 > span::before, &.arrow2 > span::after
            {
                content: "";
                position: absolute;
                height: 0;
                width:0;
                border-style: solid;
            }
            
            &.horizon
            {
                height: 2em;
                overflow: hidden;
                @each $size, $num in $sizes 
                {
                    &.#{$size}
                    {
                        width: calc(2em * $num);
                    }
                }
                &::before
                {
                    background-color: $arrow-color;
                    position: absolute;
                    top: 50%;
                    left: calc((2em + $arrow-size) / 2) ;
                    width: calc(100% - 2em - $arrow-size);
                    height:calc(2px * var(--cube-scale));
                    margin-top: 0px;
                    content: "";
                }
                &.arrow1 > span::before
                {
                    top: calc(50% - 0.25em);
                    left: calc((2em + $arrow-size) / 2 + 2px * var(--cube-scale));
                    border-top: 0.3em solid transparent;
                    border-bottom: 0.3em solid transparent;
                    border-right: 0.4em solid $arrow-color;
                    border-left: 0;
                }
                &.arrow2 > span::after
                {
                    top: calc(50% - 0.25em);
                    right: calc((2em + $arrow-size) / 2 - 2px * var(--cube-scale));
                    border-top: 0.3em solid transparent;
                    border-bottom: 0.3em solid transparent;
                    border-left: 0.4em solid $arrow-color;
                    border-right: 0;
                }
            }
            &.vertical
            {
                height: 2em;
                width: 2em;
                @each $size, $num in $sizes 
                {
                    &.#{$size}
                    {
                        height: calc(2em * $num);
                    }
                }
                &::before
                {
                    background-color: $arrow-color;
                    position: absolute;
                    left: 50%;
                    top: calc((2em + $arrow-size) / 2) ;
                    height: calc(100% - 2em - $arrow-size);
                    width:calc(2px * var(--cube-scale));
                    margin-top: 0px;
                    content: "";
                }
                &.arrow1 > span::before
                {
                    left: calc(50% - 0.25em );
                    top: calc((2em + $arrow-size) / 2 - 2px * var(--cube-scale));
                    border-left: 0.3em solid transparent;
                    border-right: 0.3em solid transparent;
                    border-bottom: 0.4em solid $arrow-color;
                    border-top: 0;
                }
                &.arrow2 > span::after
                {
                    left: calc(50% - 0.25em);
                    bottom: calc((2em + $arrow-size) / 2 - 2px * var(--cube-scale));
                    border-left: 0.3em solid transparent;
                    border-right: 0.3em solid transparent;
                    border-top: 0.4em solid $arrow-color;
                    border-bottom: 0;
                }
            }

            &.upper
            {
                @each $size, $num in $sizes 
                {
                    &.#{$size}
                    {
                        height: calc(2em * $num);
                        width: calc(2em * $num);
                        transform: translateY(calc(-2em * $num + 2em));
                    }
                }

                &::before
                {
                    background-color: $arrow-color;
                    position: absolute;
                    left: 50%;
                    top: calc((100% - (100% - 2em - $arrow-size) * 1.2 ) / 2);
                    height: calc((100% - 2em - $arrow-size) * 1.2);
                    width: calc(2px * var(--cube-scale));
                    transform: rotate(45deg);
                    margin-top: 0px;
                    content: "";
                }
                &.arrow1 > span::before
                {
                    left: calc(50% - (0.25em) - ((100% - 2em - $arrow-size) * 1.2 / 2 / 1.414));
                    bottom: calc(50% - (0.4em / 2) - ((100% - 2em - $arrow-size) * 1.2 / 2 / 1.414));
                    border-left: 0.3em solid transparent;
                    border-right: 0.3em solid transparent;
                    border-top: 0.4em solid $arrow-color;
                    border-bottom: 0;
                    transform: rotate(45deg);
                }
                &.arrow2 > span::after
                {
                    left: calc(50% - (0.25em) + ((100% - 2em - $arrow-size) * 1.2 / 2 / 1.414));
                    top: calc(50% - (0.4em / 2) - ((100% - 2em - $arrow-size) * 1.2 / 2 / 1.414));
                    border-left: 0.3em solid transparent;
                    border-right: 0.3em solid transparent;
                    border-bottom: 0.4em solid $arrow-color;
                    border-top: 0;
                    transform: rotate(45deg);
                }
            }
            &.lower
            {
                @each $size, $num in $sizes 
                {
                    &.#{$size}
                    {
                        height: calc(2em * $num);
                        width: calc(2em * $num);
                    }
                }

                &::before
                {
                    background-color: $arrow-color;
                    position: absolute;
                    left: 50%;
                    top: calc((100% - (100% - 2em - $arrow-size) * 1.1) / 2);
                    height: calc((100% - 2em - $arrow-size) * 1.1);
                    width:calc(2px * var(--cube-scale));
                    transform: rotate(-45deg);
                    margin-top: 0px;
                    content: "";
                }
                &.arrow1 > span::before
                {
                    left: calc(50% - (0.25em) - ((100% - 2em - $arrow-size) * 1.2 / 2 / 1.414));
                    top: calc(50% - (0.4em / 2) - ((100% - 2em - $arrow-size) * 1.2 / 2 / 1.414));
                    border-left: 0.3em solid transparent;
                    border-right: 0.3em solid transparent;
                    border-bottom: 0.4em solid $arrow-color;
                    border-top: 0;
                    transform: rotate(-45deg);
                }
                &.arrow2 > span::after
                {
                    left: calc(50% - (0.25em) + ((100% - 2em - $arrow-size) * 1.2 / 2 / 1.414));
                    bottom: calc(50% - (0.4em / 2) - ((100% - 2em - $arrow-size) * 1.2 / 2 / 1.414));
                    border-left: 0.3em solid transparent;
                    border-right: 0.3em solid transparent;
                    border-top: 0.4em solid $arrow-color;
                    border-bottom: 0;
                    transform: rotate(-45deg);
                }
            }
        }
    }
</style>
