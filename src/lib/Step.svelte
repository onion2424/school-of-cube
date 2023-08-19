<script lang="ts">
    let face = ["none", "blue", "orange", "white", "red", "yellow", "green", "purple"];
    export let notation = "";
    export let colors = new Array<number>(27);

</script>

<div class="step">
    <div class="scene {notation}">
        <span style="display: none;">180°</span>
        <div
            class="pivot centered"
            style="transform: rotateX(-35deg) rotateY(315deg)"
        >
            <div class="cube">
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateX(1em);"
                >
                    <div class="element right E Y'">
                        <div class="sticker {face[colors[22]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateY(-1em);"
                >
                    <div class="element top">
                        <div class="sticker {face[colors[4]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateZ(1em);"
                >
                    <div class="element front E' Y">
                        <div class="sticker {face[colors[13]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateX(1em) translateY(-1em);"
                >
                    <div class="element right U' Y'">
                        <div class="sticker {face[colors[19]]}" />
                    </div>
                    <div class="element top">
                        <div class="sticker {face[colors[5]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateY(-1em) translateZ(-1em);"
                >
                    <div class="element top">
                        <div class="sticker {face[colors[1]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateY(1em) translateZ(1em);"
                >
                    <div class="element front D' D2 Y">
                        <div class="sticker {face[colors[16]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateZ(-1em) translateX(1em);"
                >
                    <div class="element right E Y'">
                        <div class="sticker {face[colors[23]]} E" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateZ(1em) translateX(-1em);"
                >
                    <div class="element front L L' E' Y">
                        <div class="sticker {face[colors[12]]} E'" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateX(-1em) translateY(-1em);"
                >
                    <div class="element top">
                        <div class="sticker {face[colors[3]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateX(1em) translateY(1em);"
                >
                    <div class="element right D D2 Y'">
                        <div class="sticker {face[colors[25]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateY(-1em) translateZ(1em);"
                >
                    <div class="element top">
                        <div class="sticker {face[colors[7]]}" />
                    </div>
                    <div class="element front U Y">
                        <div class="sticker {face[colors[10]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateZ(1em) translateX(1em);"
                >
                    <div class="element right F F' E Y'">
                        <div class="sticker {face[colors[21]]}" />
                    </div>
                    <div class="element front R R' E' Y">
                        <div class="sticker {face[colors[14]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateX(-1em) translateY(-1em) translateZ(-1em);"
                >
                    <div class="element left">
                        <div class="sticker blue" />
                    </div>

                    <div class="element top">
                        <div class="sticker {face[colors[0]]}" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateX(1em) translateY(1em) translateZ(1em);"
                >
                    <div class="element right F F' D D2 Y'">
                        <div class="sticker {face[colors[24]]} F" />
                    </div>

                    <div class="element front R R' D' D2">
                        <div class="sticker {face[colors[17]]} R'" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateY(-1em) translateZ(1em) translateX(-1em);"
                >
                    <div class="element top">
                        <div class="sticker {face[colors[6]]}" />
                    </div>

                    <div class="element front U L L' Y'">
                        <div class="sticker {face[colors[9]]} U L'" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateY(1em) translateZ(-1em) translateX(1em);"
                >
                    <div class="element right D D2 Y'">
                        <div class="sticker {face[colors[26]]} D" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateZ(1em) translateX(1em) translateY(-1em);"
                >
                    <div class="element right U' F F' Y'">
                        <div class="sticker {face[colors[18]]} F'" />
                    </div>
                    <div class="element top">
                        <div class="sticker {face[colors[8]]}" />
                    </div>
                    <div class="element front U R R' Y">
                        <div class="sticker {face[colors[11]]} R" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateX(-1em) translateY(1em) translateZ(1em);"
                >
                    <div class="element front L L' D' D2 Y">
                        <div class="sticker {face[colors[15]]} L D'" />
                    </div>
                </div>
                <div
                    class="piece"
                    style="transform: rotateX(0deg) translateX(1em) translateY(-1em) translateZ(-1em);"
                >
                    <div class="element right U' Y'">
                        <div class="sticker {face[colors[20]]} U'" />
                    </div>
                    <div class="element top">
                        <div class="sticker {face[colors[2]]}" />
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div style="text-align: center;">{notation}</div>
</div>

<style lang="scss">
    $base-color: #0a0a0a;
    $ground-color: #2f2f31;
    $element-size: 1em;
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

    .step {
        height: auto;
        width: auto;
        position: relative;
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

    // 遷移用に矢印をつける
    :global(.arrow) .step::before
    {
        content:"→";
        position: absolute;
        left: calc(0% - 0.5em);
        top: calc((170px * var(--cube-scale)) / 4 - 0.5em);
    }

    .scene {
        height: calc(170px * var(--cube-scale) / 2);
        width: calc(170px * var(--cube-scale) / 2);
        perspective: 1200px;
        transform-style: preserve-3d;
        margin: auto;
        // &::after
        // {
        //     content:"→";
        //     position: absolute;
        //     right: calc(0% - 0.5em);
        //     top: calc(50% - 0.5em);
        // }
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
            transform-style: inherit;
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
                @each $face, $angles in $faces {
                    &.#{$face} {
                        transform: rotateX +
                            "(" +
                            nth($angles, 1) +
                            "deg)"
                            rotateY +
                            "(" +
                            nth($angles, 2) +
                            "deg)"
                            rotateZ +
                            "(" +
                            nth($angles, 3) +
                            "deg)"
                            translateZ(calc($element-size / 2));
                    }
                }
                > :global(.sticker) {
                    @extend .centered;
                    transform: translateZ(calc(1px * var(--cube-scale)));
                    width: $sticker-size;
                    height: $sticker-size;
                    border-radius: $rounded;
                    position: relative;
                    outline: 1px solid transparent; // firefox aliasing
                    box-shadow: inset 0.05em 0.05em 0.2rem 0 rgba(white, 0.25),
                        inset -0.05em -0.05em 0.2rem 0 rgba(black, 0.25);
                }
            }
        }
    }
    .scene {
        &.U2, &.D2{
            span {
                display: block !important;
                color: red;
                font-size: calc(.5em * var(--cube-scale));
                display: block;
                transform: translateZ(5px);
                text-align: left;
            }
        }
        &.U div.element.U > .sticker:before,
        &.U2 div.element.U > .sticker:before,
        &.E\' div.element.E\' > .sticker:before,
        &.D\' div.element.D\' > .sticker:before,
        &.D2 div.element.D\' > .sticker:before,
        &.Y div.element.U > .sticker:before,
        &.Y div.element.E\' > .sticker:before,
        &.Y div.element.D\' > .sticker:before,
        &.F div.element.F > .sticker::before,
        &.F\' div.element.F\' > .sticker::before
        {
            background-color: blue;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 100%;
            height: calc(2px * var(--cube-scale));
            margin-top: 0px;
            content: "";
        }

        &.U div.element.U > .sticker.U::after,
        &.U2 div.element.U > .sticker.U::after,
        &.E\' div.element.E\' > .sticker.E\'::after,
        &.D\' div.element.D\' > .sticker.D\':after,
        &.Y div.element.U > .sticker.U::after,
        &.Y div.element.E\' > .sticker.E\'::after,
        &.Y div.element.D\' > .sticker.D\':after,
        &.F\' div.element.F\' > .sticker.F\'::after
        {
            position: absolute;
            top: 50%;
            left: calc(0.5em / 1.414);
            width: .5em;
            height: .5em;
            transform: translate(-50%, -50%) rotate(-130deg);
            border-top: calc(2px * var(--cube-scale)) solid blue;
            border-right: calc(2px * var(--cube-scale)) solid blue;
            content: "";
        }

        &.U\' div.element.U\' > .sticker:before,
        &.U2 div.element.U\' > .sticker:before,
        &.E div.element.E > .sticker:before,
        &.D div.element.D > .sticker:before,
        &.D2 div.element.D > .sticker:before,
        &.Y\' div.element.U\' > .sticker:before,
        &.Y\' div.element.E > .sticker:before,
        &.Y\' div.element.D > .sticker:before
        {
            background-color: blue;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            height: 100%;
            width: calc(2px * var(--cube-scale));
            margin-top: 0px;
            content: "";
        }

        &.U\' div.element.U\' > .sticker.U\':after,
        &.D div.element.D > .sticker.D:after,
        &.D2 div.element.D > .sticker.D:after,
        &.R div.element.R > .sticker.R::after,
        &.L\' div.element.L\' > .sticker.L\'::after,
        &.E div.element.E > .sticker.E::after,
        &.Y\' div.element.U\' > .sticker.U\'::after,
        &.Y\' div.element.E > .sticker.E::after,
        &.Y\' div.element.D > .sticker.D::after
        {
            position: absolute;
            top: 50%;
            left: calc(0.5em / 1.414);
            width: .5em;
            height: .5em;
            transform: translate(-50%, -50%) rotate(-130deg);
            border-bottom: calc(2px * var(--cube-scale)) solid blue;
            border-right: calc(2px * var(--cube-scale)) solid blue;
            content: "";
        }

        &.R div.element.R > .sticker::before,
        &.R\' div.element.R\' > .sticker::before,
        &.L div.element.L > .sticker::before,
        &.L\' div.element.L\' > .sticker::before
        {
            background-color: blue;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            height: 100%;
            width: calc(2px * var(--cube-scale));
            margin-top: 0px;
            content: "";
        }



        &.R\' div.element.R\' > .sticker.R\'::after,
        &.L div.element.L > .sticker.L::after
        {
            position: absolute;
            top: 50%;
            left: calc(0.5em / 1.414);
            width: .5em;
            height: .5em;
            transform: translate(-50%, -50%) rotate(-130deg);
            border-top: calc(2px * var(--cube-scale)) solid blue;
            border-left: calc(2px * var(--cube-scale)) solid blue;
            content: "";
        }

        &.F div.element.F > .sticker.F::after
        {
            position: absolute;
            top: 50%;
            left: calc(0.5em / 1.414);
            width: .5em;
            height: .5em;
            transform: translate(-50%, -50%) rotate(-130deg);
            border-bottom: calc(2px * var(--cube-scale)) solid blue;
            border-left: calc(2px * var(--cube-scale)) solid blue;
            content: "";
        }
    }
    
</style>
