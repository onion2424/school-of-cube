<script lang="ts">
  import Step from "./lib/Step.svelte";
  import Face from "./lib/Face.svelte";
  let show = -1;
</script>

<main>
  <div id="param0">
    <h1 role="button" tabindex=0 on:click={(e) => {show = show === 0 ? -1 : 0;}} on:keyup={(e) => {return;}}><a href="#param0">0. キューブの基本</a></h1>
    {#if show === 0}
    <h2>キューブの形</h2>
    <p>3種類の形のキューブで構成されている。</p>
    <div style="display: grid; grid-template-columns: repeat(3, 1fr);">
      <div style="text-align: center">
        <Step colors={[
          0, 0, 0, 0, 7, 0, 0, 0, 0,

          0, 0, 0, 0, 7, 0, 0, 0, 0,

          0, 0, 0, 0, 7, 0, 0, 0, 0,
        ]}/>
        センターキューブ
      </div>
    <div style="text-align: center">
      <Step colors={[
        7, 0, 7, 0, 0, 0, 7, 0, 7,

        7, 0, 7, 0, 0, 0, 7, 0, 7,

        7, 0, 7, 0, 0, 0, 7, 0, 7,
      ]}/>
      コーナーキューブ
    </div>
    <div style="text-align: center">
      <Step colors={[
        0, 7, 0, 7, 0, 7, 0, 7, 0,

        0, 7, 0, 7, 0, 7, 0, 7, 0,

        0, 7, 0, 7, 0, 7, 0, 7, 0,
      ]}/>
      エッジキューブ
      </div>
    </div>
    <p>いろいろな方向に回転させてみよう！</p>
    <p>センターキューブはセンターキューブ、コーナーキューブはコーナーキューブ、エッジキューブはエッジキューブの位置にしか移動しないことがわかるはず！</p>
    <h2>回転記号</h2>
    <figure>
      <img src="https://storage.googleapis.com/tribox/solution/notations/ichiran5.png" alt="" style="height:100%;width:100%">
      <figcaption>出典：<cite><a href="https://tribox.com/3x3x3/solution/notation/">TORIBO</a><cite><figcaption>
    </figure>
    <h3>読み方(例)</h3>
    <p>
    U(ユー)
    U'(ユープライム)
    U2(ユーツー)
    Uw(ユーダブリュー)
    </p>
    <h3>上とか右という覚え方は上達を妨げる！</h3>
    <p>
      最終的には感覚で回せるようになるので、覚え方はそこまで関係ないが<br>
      上とか右では回し方をあいまいに覚えてしまいがちなので初めのうちからしっかりと回転記号で覚えよう！
    </p>  
    <h2>キューブの回し方</h2>
    <h3>上面の回し方(U, U')</h3>
    <div style="display: grid; grid-template-columns: repeat(2, 1fr);">
      <iframe width="100%" height="315" src="https://www.youtube.com/embed/rcpjD1QvIOk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      <iframe width="100%" height="315" src="https://www.youtube.com/embed/HZzvgxkzGeA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      <Step colors={[
        6, 6, 6, 6, 6, 6, 6, 6, 6,
  
        3, 3, 3, 3, 3, 3, 3, 3, 3,
  
        2, 2, 2, 2, 2, 2, 2, 2, 2,
      ]} notation="U"/>
      <Step colors={[
        6, 6, 6, 6, 6, 6, 6, 6, 6,
  
        3, 3, 3, 3, 3, 3, 3, 3, 3,
  
        2, 2, 2, 2, 2, 2, 2, 2, 2,
      ]} notation="U'"/>
    </div>
    <h3>右面の回し方(R, R')</h3>
    <div style="display: grid; grid-template-columns: repeat(2, 1fr;">
      <iframe width="100%" height="315" src="https://www.youtube.com/embed/jt8ZcRDsD4w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>      
      <iframe width="100%" height="315" src="https://www.youtube.com/embed/KlDxGaPs3gE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      <Step colors={[
        6, 6, 6, 6, 6, 6, 6, 6, 6,
  
        3, 3, 3, 3, 3, 3, 3, 3, 3,
  
        2, 2, 2, 2, 2, 2, 2, 2, 2,
      ]} notation="R"/>
      <Step colors={[
        6, 6, 6, 6, 6, 6, 6, 6, 6,
  
        3, 3, 3, 3, 3, 3, 3, 3, 3,
  
        2, 2, 2, 2, 2, 2, 2, 2, 2,
      ]} notation="R'"/>
    </div>
    <p>左面の回し方(L, L')</p>
    <div style="display: grid; grid-template-columns: repeat(2, 1fr;">
      <iframe width="100%" height="315" src="https://www.youtube.com/embed/t6KvIKSponE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      <iframe width="100%" height="315" src="https://www.youtube.com/embed/DsKX1M5akRM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    <Step colors={[
      6, 6, 6, 6, 6, 6, 6, 6, 6,

      3, 3, 3, 3, 3, 3, 3, 3, 3,

      2, 2, 2, 2, 2, 2, 2, 2, 2,
    ]} notation="L"/>
    <Step colors={[
      6, 6, 6, 6, 6, 6, 6, 6, 6,

      3, 3, 3, 3, 3, 3, 3, 3, 3,

      2, 2, 2, 2, 2, 2, 2, 2, 2,
    ]} notation="L'"/>
    </div>

    <p>最初はこのくらいを意識しよう！</p>
    {/if}
  </div>
  <div id="param1">
    <h1><a href="#param1" on:click={(e) => {show = show === 1 ? -1 : 1;}}>1. クロスをそろえる</a></h1>
    {#if show === 1}
    <Step colors={[
      0, 1, 0, 1, 1, 1, 0, 1, 0,

      0, 2, 0, 0, 2, 0, 0, 0, 0,

      0, 3, 0, 0, 3, 0, 0, 0, 0,
    ]}/>
  <p>このサイトでは青面を最初にそろえる方法で進めていく。</p>
  <Face colors={[
    1, 1, 1, 
    1, 1, 1, 
    1, 1, 1,

    2, 2, 2, 
    5, 5, 5, 
    4, 4, 4,
    3, 3, 3, 
  ]}/>
  <p>青を上面としたとき、側面は上から時計回りに「オレンジ」「黄」「赤」「白」となっている（公式の配色の場合）。</p>
  <p>実際に、青を上に向けて側面のセンターキューブを見てもらえば分かるはず。</p>
  <p>ついでにここで、「青 - 緑」「赤 - オレンジ」「白 - 黄」のセンターキューブは必ず真反対に位置することを知っておこう！
  </p>
  <h2>「おきあし」</h2>
  <p>おきあしという言葉を覚えよう。</p>
  <p>「おれんじ」「き」「あか」「しろ」の頭文字をとっておきあし！</p>
  <p>最初のうちはおきあしの順で青面のクロスを完成させていこう。<br>慣れてきたらどの順番でもOK！！</p>
  <h2>STEP1</h2>
  <p>側面がオレンジのキューブをはめる。</p>
  <Face colors={[
    0, 1, 0, 
    0, 1, 0, 
    0, 0, 0,

    0, 2, 0, 
    0, 0, 0, 
    0, 0, 0,
    0, 0, 0, 
  ]}/>
  <h2>STEP2</h2>
  <p>側面が黄のキューブをはめる。</p>
  <Face colors={[
    0, 1, 0, 
    0, 1, 1, 
    0, 0, 0,

    0, 2, 0, 
    0, 5, 0, 
    0, 0, 0,
    0, 0, 0, 
  ]}/>
  <p>STEP1ではめたキューブの次の位置(時計回り)にはめる！</p>
  <h2>STEP3</h2>
  <p>側面が赤のキューブをはめる。</p>
  <Face colors={[
    0, 1, 0, 
    0, 1, 1, 
    0, 1, 0,

    0, 2, 0, 
    0, 5, 0, 
    0, 4, 0,
    0, 0, 0, 
  ]}/>
  <p>STEP2ではめたキューブの次の位置(時計回り)にはめる！</p>
  <h2>STEP4</h2>
  <p>側面が白のキューブをはめる。</p>
  <Face colors={[
    0, 1, 0, 
    1, 1, 1, 
    0, 1, 0,

    0, 2, 0, 
    0, 5, 0, 
    0, 4, 0,
    0, 3, 0, 
  ]}/>
  <p>STEP3ではめたキューブの次の位置(時計回り)にはめる！</p>
  <h2>回し方</h2>
  <h3>2種類の入れ方を覚える！</h3>
  <div style="display: grid; grid-template-columns: repeat(2, 1fr);">
    <div >
      <Step colors={[
        0, 1, 0, 1, 1, 1, 0, 0, 0,

        0, 0, 0, 0, 2, 2, 0, 0, 0,

        0, 3, 0, 1, 3, 0, 0, 0, 0,
      ]} notation="F'"/>
    </div>
  <div >
    <Step colors={[
      0, 1, 0, 1, 1, 0, 0, 1, 0,

      0, 2, 0, 0, 2, 1, 0, 0, 0,

      0, 0, 0, 3, 3, 0, 0, 0, 0,
    ]} notation="R"/>
  </div>

</div>
<h3>2段目に無い場合は1度回すと2段目にくる！</h3>
<div style="display: grid; grid-template-columns: repeat(4, 1fr);">
  <div >
    <Step colors={[
        0, 1, 0, 1, 1, 1, 0, 7, 0,

        0, 7, 0, 0, 2, 0, 0, 7, 0,

        0, 3, 0, 0, 3, 0, 0, 0, 0,
    ]} notation="F"/>
  </div>
  <div >
    <Step colors={[
      0, 1, 0, 1, 1, 1, 0, 0, 0,
       
      0, 0, 0, 7, 2, 7, 0, 0, 0,

      0, 3, 0, 7, 3, 0, 0, 0, 0,
    ]}/>
  </div>
  <div>
    <Step colors={[
      0, 1, 0, 1, 1, 7, 0, 1, 0,

      0, 2, 0, 0, 2, 0, 0, 0, 0,

      0, 7, 0, 0, 3, 0, 0, 7, 0,
    ]} notation="R"/>
  </div>
  <div class="arrow">
    <Step colors={[
      0, 1, 0, 1, 1, 0, 0, 1, 0,

      0, 2, 0, 0, 2, 7, 0, 0, 0,

      0, 0, 0, 7, 3, 7, 0, 0, 0,
    ]}/>
  </div>
</div>
{/if}
</div>
  <div id="param2">
    <h1 on:click={(e) => {show = show === 2 ? -1 : 2;}}><a href="#param2">2. コーナーキューブを入れて一面をそろえる</a></h1>
    {#if show === 2}
    <Step colors={[
      1, 1, 1, 1, 1, 1, 1, 1, 1,

      2, 2, 2, 0, 2, 0, 0, 0, 0,

      3, 3, 3, 0, 3, 0, 0, 0, 0,
    ]}/>
    <h2>ポイント！</h2>
    <p>入れようとしているキューブを、入れたい位置の真下に持ってこよう！</p>
    <p>例えば...</p>
    <div style="display: grid; grid-template-columns: repeat(4, 1fr);">
      <div style="text-align: center">
        ピンクに入れたいから
        <Step colors={[
          1, 1, 1, 1, 1, 1, 1, 1, 7,

          2, 2, 7, 0, 2, 0, 1, 0, 0,

          7, 3, 3, 0, 3, 0, 0, 0, 0,
        ]} notation="D"/>
      </div>
      <div class="arrow" style="text-align: center">
        真下に持ってくる！
        <Step colors={[
          1, 1, 1, 1, 1, 1, 1, 1, 7,

          2, 2, 7, 0, 2, 0, 0, 0, 2,

          7, 3, 3, 0, 3, 0, 1, 0, 0,
        ]}/>
      </div>
      <div style="text-align: center">
        ピンクに入れたいから
        <Step colors={[
          1, 1, 1, 1, 1, 1, 1, 1, 7,

          2, 2, 7, 0, 2, 0, 0, 0, 0,

          7, 3, 3, 0, 3, 0, 0, 0, 3,
        ]} notation="D'"/>
      </div>
      <div class="arrow" style="text-align: center">
        真下に持ってくる！
        <Step colors={[
          1, 1, 1, 1, 1, 1, 1, 1, 7,

          2, 2, 7, 0, 2, 0, 0, 0, 3,

          7, 3, 3, 0, 3, 0, 1, 0, 0,
        ]}/>
      </div>
    </div>
    <p>真下に持ってこられたら、入れるための回し方を覚えよう！</p>

    <h2>回し方</h2>
    <h3>2種類の入れ方を覚える！</h3>
    <p>真下に持ってきたコーナーキューブの青面を自分にむけると、この2つのどちらかになる！</p>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
      <div>
        <Step colors={[
          1, 1, 1, 1, 1, 1, 1, 1, 0,
  
          2, 2, 0, 0, 2, 0, 0, 0, 1,
  
          0, 3, 3, 0, 3, 0, 3, 0, 0,
        ]} notation="R"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 1, 0, 1, 1, 0, 1, 1, 1,
  
          2, 2, 2, 0, 2, 0, 0, 0, 0,
  
          3, 0, 0, 0, 3, 3, 0, 0, 3,
        ]} notation="F'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 1, 0, 1, 1, 0, 3, 0, 0,
  
          2, 0, 0, 2, 2, 0, 2, 0, 0,
  
          0, 0, 0, 0, 3, 3, 0, 0, 3,
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 1, 1, 1, 1, 1, 3, 0, 0,
  
          2, 0, 0, 2, 2, 0, 2, 0, 0,
  
          0, 3, 3, 0, 3, 0, 0, 0, 0,
        ]} notation="F"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 1, 1, 1, 1, 1, 1, 1, 1,
    
          2, 2, 2, 0, 2, 0, 0, 0, 0,
    
          3, 3, 3, 0, 3, 0, 0, 0, 0,
        ]}/>
      </div>
    </div>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
        <div>
          <Step colors={[
            1, 1, 1, 1, 1, 1, 0, 1, 1,
    
            0, 2, 2, 0, 2, 0, 1, 0, 0,
    
            3, 3, 3, 0, 3, 3, 0, 0, 0,
          ]} notation="L'"/>
        </div>
        <div class="arrow">
          <Step colors={[
            0, 1, 1, 0, 1, 1, 1, 1, 1,
    
            2, 2, 2, 0, 2, 0, 0, 0, 0,
    
            3, 3, 3, 0, 3, 3, 0, 0, 0,
          ]} notation="F"/>
        </div>
        <div class="arrow">
          <Step colors={[
            0, 1, 1, 0, 1, 1, 0, 0, 3,
    
            0, 0, 2, 0, 2, 2, 0, 0, 2,
    
            1, 3, 3, 1, 3, 3, 1, 0, 0,
          ]} notation="L"/>
        </div>
        <div class="arrow">
          <Step colors={[
            1, 1, 1, 1, 1, 1, 0, 0, 3,
    
            0, 0, 2, 0, 2, 2, 0, 0, 2,
    
            1, 3, 3, 1, 3, 3, 1, 0, 0,
          ]} notation="F'"/>
        </div>
        <div class="arrow">
          <Step colors={[
            1, 1, 1, 1, 1, 1, 1, 1, 1,
      
            2, 2, 2, 0, 2, 0, 0, 0, 0,
      
            3, 3, 3, 0, 3, 0, 0, 0, 0,
          ]}/>
        </div>
    </div>
    <p>どちらの回し方でも、最初の1手で入れたい位置にぴったりくる！</p>
    <h3>下を向いてしまっている場合</h3>
    <p>次の手順を行い、向きを変えてあげよう！</p>
    <div style="display: grid; grid-template-columns: repeat(4, 1fr);">
      <div>
        <Step colors={[
          1, 1, 1, 1, 1, 1, 1, 1, 0,
  
          2, 2, 0, 0, 2, 0, 0, 0, 3,
  
          0, 3, 3, 0, 3, 0, 2, 0, 0,
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 1, 0, 1, 1, 0, 1, 1, 4,
  
          2, 2, 1, 0, 2, 1, 0, 0, 0,
  
          3, 0, 0, 3, 3, 0, 0, 0, 2,
        ]} notation="D2"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 1, 0, 1, 1, 0, 1, 1, 4,
  
          2, 2, 1, 0, 2, 1, 1, 0, 0,
  
          3, 0, 0, 3, 3, 0, 0, 0, 0,
        ]} notation="R"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 1, 1, 1, 1, 1, 1, 1, 0,
  
          2, 2, 0, 0, 2, 0, 1, 0, 0,
  
          0, 3, 3, 0, 3, 0, 0, 0, 0,
        ]}/>
      </div>
    </div>
    <h3>違う位置に入ってしまっている場合</h3>
    <p>適当なキューブを入れてあげよう！</p>
    <div style="display: grid; grid-template-columns: repeat(2, 1fr);">
      <div>
        <Step colors={[
          0, 1, 1, 1, 1, 1, 1, 1, 1,
    
          2, 2, 4, 0, 2, 0, 0, 0, 0,
    
          5, 3, 3, 0, 3, 0, 0, 0, 0,
        ]}/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 1, 1, 1, 1, 1, 1, 1, 2,
    
          2, 2, 6, 0, 2, 0, 0, 0, 0,
    
          3, 3, 3, 0, 3, 0, 0, 0, 0,
        ]}/>
      </div>
    </div>
    {/if}
  </div>
  <div id="param3">
    <h1 on:click={(e) => {show = show === 3 ? -1 : 3;}}><a href="#param3">3. 2列目をそろえる</a></h1>
    {#if show === 3}
    <Step colors={[
      0, 0, 0, 0, 6, 0, 0, 0, 0,

      0, 0, 0, 3, 3, 3, 3, 3, 3, 

      0, 0, 0, 2, 2, 2, 2, 2, 2, 

    ]}/>
    <h2>一面をそろえられたら、すぐ下に向ける！</h2>
    <p>これ以降は緑が上面で進めていくよ！</p>
    <h1>ポイント</h1>
    <p>
      入れようとしているキューブを、入れたい場所の斜め上に持ってこよう！<br/>
      縦一直線同じ色になるのもポイント！
    </p>
    <div style="display: grid; grid-template-columns: repeat(4, 1fr);">
      <div style="text-align:center;">
        ピンクに入れたいから
        <Step colors={[
          0, 0, 0, 2, 6, 0, 0, 0, 0,
    
          0, 0, 0, 3, 3, 7, 3, 3, 3, 
    
          0, 0, 0, 7, 2, 2, 2, 2, 2, 
        ]} notation="U'"/>
      </div>
      <div class="arrow "style="text-align:center;">
        斜め上に持ってくる！
        <Step colors={[
          0, 0, 0, 0, 6, 0, 0, 2, 0,
    
          0, 3, 0, 3, 3, 0, 3, 3, 3, 
    
          0, 0, 0, 0, 2, 2, 2, 2, 2, 
        ]}/>
        縦一直線！
      </div>
      <div style="text-align:center;">
        ピンクに入れたいから
        <Step colors={[
          0, 0, 0, 0, 6, 0, 0, 3, 0,
    
          0, 2, 0, 3, 3, 7, 3, 3, 3, 
    
          0, 0, 0, 7, 2, 2, 2, 2, 2, 
        ]} notation="U'"/>
        縦一直線？
      </div>
      <div class="arrow "style="text-align:center;">
        斜め上に持ってくる！
        <Step colors={[
          0, 0, 0, 0, 6, 0, 0, 2, 0,
    
          0, 3, 0, 3, 3, 0, 3, 3, 3, 
    
          0, 0, 0, 0, 2, 2, 2, 2, 2, 
        ]}/>
        縦一直線！
      </div>
    </div>
    <p>2列目に入っちゃっている時がある！</p>
    <p>そういうときは、適当なキューブを入れて外に出してあげよう！</p>
    <div style="display: grid; grid-template-columns: repeat(4, 1fr);">
      <div style="text-align:center;">
        逆なら
        <Step colors={[
          0, 0, 0, 0, 6, 0, 0, 7, 0,
    
          0, 7, 0, 3, 3, 2, 3, 3, 3, 
    
          0, 0, 0, 3, 2, 2, 2, 2, 2, 
        ]}/>
        右側パターン
      </div>
      <div class="arrow "style="text-align:center;">
        外に！
        <Step colors={[
          0, 2, 0, 0, 6, 0, 0, 0, 0,
    
          0, 0, 0, 3, 3, 7, 3, 3, 3, 
    
          0, 0, 0, 7, 2, 2, 2, 2, 2, 
        ]}/>
      </div>
      <div style="text-align:center;">
        違うなら
        <Step colors={[
          0, 0, 0, 0, 6, 7, 0, 0, 0,
    
          0, 0, 0, 3, 3, 3, 3, 3, 3, 
    
          0, 7, 0, 5, 2, 2, 2, 2, 2, 
        ]}/>
        左側パターン
      </div>
      <div class="arrow "style="text-align:center;">
        外に！
        <Step colors={[
          0, 0, 0, 5, 6, 0, 0, 0, 0,
    
          0, 0, 0, 3, 3, 7, 3, 3, 3, 
    
          0, 0, 0, 7, 2, 2, 2, 2, 2, 
        ]}/>
      </div>
    </div> 
    <h2>回し方</h2>
    <h3>2種類の入れ方を覚える！</h3>
    <p>入れようとしているキューブを、センターキューブの真上に持ってくることがポイント！</p>
    <p>入れようとしているキューブを自分に向けると、この2つのどちらかになる！</p>
    <h3>入れたい場所が右側にあるパターン</h3>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
    <div>
      <Step colors={[
        0, 0, 0, 0, 6, 0, 0, 2, 0,
  
        0, 3, 0, 3, 3, 0, 3, 3, 3, 
  
        0, 0, 0, 0, 2, 2, 2, 2, 2, 
      ]} notation="U"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 0, 2, 6, 0, 0, 0, 0,
  
        0, 0, 0, 3, 3, 0, 3, 3, 3, 
  
        0, 0, 0, 0, 2, 2, 2, 2, 2, 
      ]} notation="R"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 0, 2, 6, 0, 0, 0, 3,
  
        0, 0, 1, 3, 3, 1, 3, 3, 1, 
  
        2, 0, 0, 2, 2, 0, 2, 2, 0, 
      ]} notation="U'"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 3, 0, 6, 0, 0, 2, 0,
  
        0, 3, 0, 3, 3, 1, 3, 3, 1, 
  
        0, 0, 1, 2, 2, 0, 2, 2, 0, 
      ]} notation="R'"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 0, 0, 6, 0, 0, 2, 2,
  
        0, 3, 3, 3, 3, 0, 3, 3, 0, 
  
        1, 0, 0, 0, 2, 2, 0, 2, 2, 
      ]} notation="Y"/>
    </div>
    </div>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
      <div class="arrow">
      <Step colors={[
        0, 0, 0, 2, 6, 0, 2, 0, 0,
  
        1, 0, 0, 0, 2, 2, 0, 2, 2, 
  
        0, 0, 0, 5, 5, 5, 5, 5, 5, 
      ]} notation="U'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 0, 0, 0, 6, 0, 0, 2, 2,
    
          0, 3, 3, 0, 2, 2, 0, 2, 2, 
    
          1, 0, 0, 5, 5, 5, 5, 5, 5, 
        ]} notation="L'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 0, 0, 0, 6, 0, 0, 2, 2,
    
          0, 3, 3, 1, 2, 2, 1, 2, 2, 
    
          1, 0, 0, 5, 5, 5, 5, 5, 5, 
        ]} notation="U"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 0, 0, 2, 6, 0, 2, 0, 0,
    
          1, 0, 0, 1, 2, 2, 1, 2, 2, 
    
          0, 0, 0, 5, 5, 5, 5, 5, 5, 
        ]} notation="L"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 0, 0, 0, 6, 0, 0, 0, 0,
    
          0, 0, 0, 2, 2, 2, 2, 2, 2, 
    
          0, 0, 0, 5, 5, 5, 5, 5, 5, 
        ]}/>
      </div>
    </div>
    <h3>入れたい場所が左側にあるパターン</h3>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
    <div>
      <Step colors={[
        0, 0, 0, 0, 6, 0, 0, 4, 0,
  
        0, 3, 0, 0, 3, 3, 3, 3, 3, 
  
        0, 0, 0, 2, 2, 2, 2, 2, 2, 
      ]} notation="U'"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 0, 0, 6, 4, 0, 0, 0,
  
        0, 0, 0, 0, 3, 3, 3, 3, 3, 
  
        0, 3, 0, 2, 2, 2, 2, 2, 2, 
      ]} notation="L'"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 0, 0, 6, 4, 3, 0, 0,
  
        1, 0, 0, 1, 3, 3, 1, 3, 3, 
  
        0, 3, 0, 2, 2, 2, 2, 2, 2, 
      ]} notation="U"/>
    </div>
    <div class="arrow">
      <Step colors={[
        3, 0, 0, 0, 6, 0, 0, 4, 0,
  
        0, 3, 0, 1, 3, 3, 1, 3, 3, 
  
        0, 3, 0, 2, 2, 2, 2, 2, 2, 
      ]} notation="L"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 0, 0, 6, 0, 4, 4, 0,
  
        3, 3, 0, 0, 3, 3, 0, 3, 3, 
  
        0, 0, 0, 2, 2, 2, 2, 2, 2, 
      ]} notation="Y'"/>
    </div>
    </div>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
      <div class="arrow">
      <Step colors={[
        0, 0, 0, 0, 6, 4, 0, 0, 4,
  
        0, 0, 1, 4, 4, 0, 4, 4, 0, 
  
        3, 3, 0, 0, 3, 3, 0, 3, 3, 
      ]} notation="U"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 0, 0, 0, 6, 0, 4, 4, 0,
    
          3, 3, 0, 4, 4, 0, 4, 4, 0, 
    
          0, 0, 0, 0, 3, 3, 0, 3, 3, 
        ]} notation="R"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 0, 0, 0, 6, 0, 4, 4, 0,
    
          3, 3, 0, 4, 4, 1, 4, 4, 1, 
    
          0, 0, 0, 3, 3, 0, 3, 3, 0, 
        ]} notation="U'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 0, 0, 0, 6, 4, 0, 0, 4,
    
          0, 0, 1, 4, 4, 1, 4, 4, 1, 
    
          3, 3, 0, 3, 3, 0, 3, 3, 0, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 0, 0, 0, 6, 0, 0, 0, 0,
    
          0, 0, 0, 4, 4, 4, 4, 4, 4, 
    
          0, 0, 0, 3, 3, 3, 3, 3, 3, 
        ]}/>
      </div>
    </div>
    {/if}
  </div>
  
  <div id="param4">
    <h1 on:click={(e) => {show = show === 4 ? -1 : 4;}}><a href="#param4">4. 上面のクロスをそろえる</a></h1>
    {#if show === 4}
    <Step colors={[
      0, 6, 0, 6, 6, 6, 0, 6, 0,

      0, 0, 0, 3, 3, 3, 3, 3, 3, 

      0, 0, 0, 2, 2, 2, 2, 2, 2, 
    ]}/>
    <h2>上面のエッジキューブだけに注目する！</h2>
    <p>2列目をそろえたら、上の緑面のエッジキューブだけに注目すると4パターンのどれかになっている！</p>
    <div style="display: grid; grid-template-columns: repeat(4, 1fr);">
      <div style="text-align: center">
      <Face colors={[
        7, 0, 7, 0, 6, 0, 7, 0, 7,

        0, 6, 0,
        0, 6, 0,
        0, 6, 0,
        0, 6, 0, 
      ]} classes={["horizon location6 size3  arrow2"]}/>
      点
      </div>
      <div style="text-align: center">
        <Face colors={[
          7, 0, 7, 0, 6, 6, 7, 6, 7,
  
          0, 6, 0,
          0, 0, 0,
          0, 0, 0,
          0, 6, 0, 
        ]} classes={["horizon location6 size3  arrow2"]}/>
        くの字
      </div>
      <div style="text-align: center">
        <Face colors={[
          7, 0, 7, 6, 6, 6, 7, 0, 7,
  
          0, 6, 0,
          0, 0, 0,
          0, 6, 0,
          0, 0, 0, 
        ]} classes={["horizon location6 size3  arrow2"]}/>
        直線
      </div>
      <div style="text-align: center">
        <Face colors={[
          7, 6, 7, 6, 6, 6, 7, 6, 7,
  
          0, 0, 0,
          0, 0, 0,
          0, 0, 0,
          0, 0, 0, 
        ]}/>
        クロス（完成済み）
      </div>
    </div>
    <p>向きが大事なのでこの図をしっかり覚えよう！最初は矢印の向きに回す！</p>
    <h2>回し方</h2>
    <h3>1種類の回し方を覚える！</h3>
    <p>上の図の通りの向きで回し始めることがポイント！</p>
    <p>クロスが出来るまで1～3回かかる！毎回向きをしっかり合わせよう！<br/>
    点→くの字→直線→クロスの順で出来ていく！この順に進まなかったら向きが間違っているよ！
    </p>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
    <div>
      <Step colors={[
        0, 0, 0, 6, 6, 6, 0, 0, 0,
  
        0, 6, 0, 3, 3, 3, 3, 3, 3, 
  
        0, 0, 0, 2, 2, 2, 2, 2, 2, 
      ]} notation="F"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 0, 6, 6, 6, 4, 4, 0,
  
        3, 3, 0, 3, 3, 6, 3, 3, 0, 
  
        0, 0, 0, 0, 2, 2, 0, 2, 2, 
      ]} notation="R"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 0, 0, 6, 6, 6, 4, 4, 0,
  
        3, 3, 0, 3, 3, 1, 3, 3, 1, 
  
        0, 0, 0, 2, 2, 0, 2, 2, 0, 
      ]} notation="U"/>
    </div>
    <div class="arrow">
      <Step colors={[
        4, 6, 0, 4, 6, 0, 0, 6, 0,
  
        0, 0, 0, 3, 3, 1, 3, 3, 1, 
  
        0, 6, 0, 2, 2, 0, 2, 2, 0, 
      ]} notation="R'"/>
    </div>
    <div class="arrow">
      <Step colors={[
        4, 6, 0, 4, 6, 6, 0, 6, 0,
  
        0, 0, 0, 3, 3, 0, 3, 3, 0, 
  
        0, 0, 0, 6, 2, 2, 0, 2, 2, 
      ]} notation="U'"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 6, 0, 6, 6, 6, 4, 4, 0,
  
        3, 3, 0, 3, 3, 0, 3, 3, 0, 
  
        0, 0, 0, 6, 2, 2, 0, 2, 2, 
      ]} notation="F'"/>
    </div>
    <div class="arrow">
      <Step colors={[
        0, 6, 0, 6, 6, 6, 0, 6, 0,
  
        0, 0, 0, 3, 3, 3, 3, 3, 3, 
  
        0, 0, 0, 2, 2, 2, 2, 2, 2, 
      ]}/>
    </div>
  </div>
  {/if}
  </div>
  <div id="param5">
    <h1 on:click={(e) => {show = show === 5 ? -1 : 5;}}><a href="#param5">5. 上面をそろえる</a></h1>
    {#if show === 5}
    <Step colors={[
      6, 6, 6, 6, 6, 6, 6, 6, 6,

      0, 0, 0, 3, 3, 3, 3, 3, 3, 

      0, 0, 0, 2, 2, 2, 2, 2, 2, 

    ]}/>
    <h2>上面のクロスをそろえたら、緑のキューブのみに注目すると8パターン！</h2>
    <div style="display: grid; grid-template-columns: repeat(4, 1fr); row-gap: 1.5em;">
      <div style="text-align: center">
        パターン1
      <Face colors={[
        0, 6, 6, 6, 6, 6, 0, 6, 0,

        0, 0, 0,
        0, 0, 6,
        0, 0, 6,
        0, 0, 6, 
      ]} classes={["vertical location2 size3  arrow1"]}/>
      →パターン8！
      </div>
      <div style="text-align: center">
        パターン2
        <Face colors={[
          0, 6, 6, 6, 6, 6, 0, 6, 0,
  
          6, 0, 0,
          0, 0, 0,
          6, 0, 0,
          6, 0, 0, 
        ]} classes={["vertical location2 size3  arrow1"]}/>
        →パターン1
      </div>
      <div style="text-align: center">
        パターン3
        <Face colors={[
          0, 6, 0, 6, 6, 6, 0, 6, 0,
  
          0, 0, 6,
          0, 0, 0,
          6, 0, 0,
          6, 0, 6, 
        ]} classes={["vertical location2 size3  arrow1"]}/>
        →パターン1
      </div>
      <div style="text-align: center">
        パターン4
        <Face colors={[
          0, 6, 0, 6, 6, 6, 0, 6, 0,
  
          6, 0, 6,
          0, 0, 0,
          6, 0, 6,
          0, 0, 0, 
        ]} classes={["vertical location2 size3  arrow1"]}/>
        →パターン1
      </div>
      <div style="text-align: center">
        パターン5
      <Face colors={[
        0, 6, 0, 6, 6, 6, 6, 6, 6,

        0, 0, 0,
        6, 0, 0,
        0, 0, 0,
        0, 0, 6, 
      ]} classes={["vertical location2 size3  arrow1"]}/>
      →パターン2
      </div>
      <div style="text-align: center">
        パターン6
        <Face colors={[
          6, 6, 0, 6, 6, 6, 6, 6, 0,
  
          0, 0, 0,
          6, 0, 6,
          0, 0, 0,
          0, 0, 0, 
        ]} classes={["vertical location2 size3  arrow1"]}/>
        →パターン2
      </div>
      <div style="text-align: center">
        パターン7
        <Face colors={[
          6, 6, 0, 6, 6, 6, 0, 6, 6,
  
          0, 0, 0,
          6, 0, 0,
          0, 0, 6,
          0, 0, 0, 
        ]} classes={["vertical location2 size3  arrow1"]}/>
        →パターン2
      </div>
      <div style="text-align: center">
        パターン8
        <Face colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
  
          0, 0, 0,
          0, 0, 0,
          0, 0, 0,
          0, 0, 0, 
        ]}/>
        完成
      </div>
    </div>
    <p>向きが大事なのでこの図をしっかり覚えよう！最初は矢印の向きに回す！</p>
    <h2>回し方</h2>
    <h3>1種類の回し方を覚える！</h3>
    <p>上の図の通りの向きで回し始めることがポイント！</p>
    <p>上面が完成するまで1～3回かかる！毎回向きをしっかり合わせよう！<br/>
    回した後にどのパターンになるかも書いているから、この順に進まなかった場合は向きが間違っているよ！
    </p>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
      <div>
        <Step colors={[
          0, 6, 6, 6, 6, 6, 0, 6, 0,
    
          6, 0, 0, 3, 3, 3, 3, 3, 3, 
    
          6, 0, 0, 2, 2, 2, 2, 2, 2, 
        ]} notation="R"/>
      </div>
      <div class="arrow">
        <Step colors={[
          0, 6, 0, 6, 6, 3, 0, 6, 3,
    
          6, 0, 1, 3, 3, 1, 3, 3, 1, 
    
          2, 2, 6, 2, 2, 0, 2, 2, 0, 
        ]} notation="U2"/>
      </div>
      <div class="arrow">
        <Step colors={[
          3, 6, 0, 3, 6, 6, 0, 6, 0,
    
          0, 0, 0, 3, 3, 1, 3, 3, 1, 
    
          6, 0, 0, 2, 2, 0, 2, 2, 0, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          3, 6, 6, 3, 6, 6, 0, 6, 6,
    
          0, 0, 0, 3, 3, 6, 3, 3, 0, 
    
          0, 0, 0, 0, 2, 2, 6, 2, 2, 
        ]} notation="U'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 3, 3, 0,
    
          2, 2, 6, 3, 3, 6, 3, 3, 0, 
    
          0, 0, 0, 0, 2, 2, 6, 2, 2, 
        ]} notation="R"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 3, 3, 0,
    
          2, 2, 0, 3, 3, 1, 3, 3, 1, 
    
          6, 0, 0, 2, 2, 0, 2, 2, 0, 
        ]} notation="U'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 0, 6, 6, 3, 6, 6, 3,
    
          0, 0, 1, 3, 3, 1, 3, 3, 1, 
    
          2, 2, 0, 2, 2, 0, 2, 2, 0, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 0, 0, 3, 3, 3, 3, 3, 3, 
    
          0, 0, 0, 2, 2, 2, 2, 2, 2, 
        ]}/>
      </div>
    </div>
    {/if}
    </div>
  <div id="param6">
    <h1 on:click={(e) => {show = show === 6 ? -1 : 6;}}><a href="#param6">6. エッジキューブの向きをそろえる</a></h1>
    {#if show === 6}
    <Step colors={[
      6, 6, 6, 6, 6, 6, 6, 6, 6,

      0, 3, 0, 3, 3, 3, 3, 3, 3, 

      0, 2, 0, 2, 2, 2, 2, 2, 2, 
    ]}/>
    <h2>パターンの把握が難しい！</h2>
    <p>上段をくるくる回してみよう。</p>
    <Step colors={[
      6, 6, 6, 6, 6, 6, 6, 6, 6,

      0, 0, 0, 3, 3, 3, 3, 3, 3, 

      0, 0, 0, 2, 2, 2, 2, 2, 2, 
    ]} notation="U"/>
    
    <p>くるくる回していると、センターキューブとエッジキューブがそろうときがいくつかある！</p>
    <Step colors={[
      6, 6, 6, 6, 6, 6, 6, 6, 6,

      0, 7, 0, 0, 7, 0, 0, 0, 0, 

      0, 0, 0, 0, 0, 0, 0, 0, 0, 
    ]}/>
    <p>センターキューブとエッジキューブがそろうというのは、上のキューブで言うピンクの位置の色が同じという意味だよ！
    </p>
    <p>上面を回してみて、</p>
    <div style="display: grid; grid-template-columns: repeat(4, 1fr);">
      <div style="text-align:center;">
        白
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 3, 0, 3, 3, 3, 3, 3, 3, 
    
          0, 0, 0, 2, 2, 2, 2, 2, 2, 
        ]}/>
      </div>
      <div style="text-align:center;">
        オレンジ
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 2, 0, 2, 2, 2, 2, 2, 2, 

          0, 0, 0, 5, 5, 5, 5, 5, 5, 
        ]}/>
      </div>
      <div style="text-align:center;">
        黄
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 5, 0, 5, 5, 5, 5, 5, 5, 
    
          0, 0, 0, 4, 4, 4, 4, 4, 4, 
        ]}/>
      </div>
      <div style="text-align:center;">
        赤
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,

          0, 4, 0, 4, 4, 4, 4, 4, 4, 
    
          0, 0, 0, 3, 3, 3, 3, 3, 3, 
        ]}/>
      </div>
    </div>
    <p>こんな感じで全部の色を一回ずつそろえてみよう！</p>
    <p>そろえたうちのどれかが次の3パターンに絶対に当てはまっている！</p>
    <p>どれかを見つけたら、そろっている面を奥にして次のパターンにあてはまらないか探してね！</p>
    <div style="display: grid; grid-template-columns: repeat(3, 1fr);">
      <div style="text-align: center">
      パターン1
      <Face colors={[
        6, 6, 6, 6, 6, 6, 6, 6, 6,

        0, 7, 0,
        0, 0, 0,
        0, 0, 0,
        0, 0, 0, 
      ]} classes={["vertical location2 size3  arrow1"]}/>
      1つだけそろう場合<br/>
      →パターン1, 3
      </div>
      <div style="text-align: center">
        パターン2
        <Face colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
  
          0, 7, 0,
          0, 0, 0,
          0, 7, 0,
          0, 0, 0, 
        ]} classes={["vertical location2 size3  arrow1"]}/>
        かならず2つ以上そろう場合<br/>
        →パターン1
      </div>
      <div style="text-align: center">
        パターン3
        <Face colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
  
          0, 7, 0,
          0, 7, 0,
          0, 7, 0,
          0, 7, 0, 
        ]}/>
        全部そろっている場合<br/>
        完成
      </div>
    </div>
    <h2>回し方</h2>
    <h3>1種類の回し方を覚える！</h3>
    <p>センターキューブとエッジキューブがそろっている面を奥側にすることがポイント！</p>
    <p>完成するまで1～3回かかる！毎回向きをしっかり合わせよう！</p>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
      <div>
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 4, 0, 3, 3, 3, 3, 3, 3, 
    
          0, 3, 0, 2, 2, 2, 2, 2, 2, 
        ]} notation="R2"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 1, 6, 6, 1, 6, 6, 1,
    
          0, 4, 5, 3, 3, 5, 3, 3, 0, 
    
          2, 2, 2, 2, 2, 2, 0, 3, 0, 
        ]} notation="U"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 1, 1, 1,
    
          2, 2, 2, 3, 3, 5, 3, 3, 0, 
    
          3, 5, 0, 2, 2, 2, 0, 3, 0, 
        ]} notation="R"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 2, 6, 6, 5, 1, 1, 0,
    
          2, 2, 6, 3, 3, 6, 3, 3, 6, 
    
          0, 2, 3, 3, 2, 5, 0, 2, 5, 
        ]} notation="U"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 6, 6, 1, 6, 6, 0, 5, 2,
    
          0, 2, 3, 3, 3, 6, 3, 3, 6, 
    
          1, 2, 0, 3, 2, 5, 0, 2, 5, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          1, 6, 6, 1, 6, 6, 0, 5, 0,
    
          2, 2, 6, 3, 3, 6, 3, 3, 2, 
    
          0, 5, 0, 2, 2, 2, 1, 3, 0, 
        ]} notation="U'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 0, 6, 6, 5, 1, 1, 0,
    
          2, 2, 6, 3, 3, 6, 3, 3, 2, 
    
          0, 2, 6, 2, 2, 2, 1, 3, 0, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 0, 6, 6, 3, 1, 1, 0,
    
          2, 2, 0, 3, 3, 5, 3, 3, 0, 
    
          6, 2, 0, 2, 2, 3, 0, 2, 1, 
        ]} notation="U'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          3, 3, 0, 6, 6, 1, 6, 6, 1,
    
          0, 4, 5, 3, 3, 5, 3, 3, 0, 
    
          2, 2, 0, 2, 2, 3, 0, 2, 1, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          3, 3, 3, 6, 6, 6, 6, 6, 6,
    
          0, 4, 0, 3, 3, 1, 3, 3, 1, 
    
          0, 3, 1, 2, 2, 2, 2, 2, 0, 
        ]} notation="U"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 3, 6, 6, 3, 6, 6, 3,
    
          0, 3, 1, 3, 3, 1, 3, 3, 1, 
    
          2, 2, 0, 2, 2, 2, 2, 2, 0, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 3, 0, 3, 3, 3, 3, 3, 3, 
    
          0, 2, 0, 2, 2, 2, 2, 2, 2, 
        ]}/>
      </div> 
    </div>
    {/if}
  </div>
  <div id="param7">
    <h1 on:click={(e) => {show = show === 7 ? -1 : 7;}}><a href="#param7">7. コーナーキューブの向きをそろえる</a></h1>
    {#if show === 7}
    <Step colors={[
      6, 6, 6, 6, 6, 6, 6, 6, 6,

      3, 3, 3, 3, 3, 3, 3, 3, 3, 

      2, 2, 2, 2, 2, 2, 2, 2, 2, 
    ]}/>
    <h2>そろっているコーナーキューブを探そう！</h2>
    <p>一つ前の手順を終えてエッジキューブがそろったら、次はそろっているコーナーキューブを探そう！</p>
    <div style="display: grid; grid-template-columns: repeat(4, 1fr);">
      <div style="text-align:center;">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 3, 3, 3, 3, 3, 3, 3, 3,

          2, 2, 0, 2, 2, 2, 2, 2, 2, 
        ]}/>
        これ？
      </div>
      <div style="text-align:center;">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 4, 4, 4, 4, 4, 4, 4, 4, 
    
          3, 3, 0, 3, 3, 3, 3, 3, 3, 
        ]}/>
        それ？
      </div>
      <div style="text-align:center;">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 5, 5, 5, 5, 5, 5, 5, 5, 
    
          4, 4, 0, 4, 4, 4, 4, 4, 4, 
        ]}/>
        あれ？
      </div>
      <div style="text-align:center;">
        <Step colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
    
          0, 2, 2, 2, 2, 2, 2, 2, 2, 

          5, 5, 0, 5, 5, 5, 5, 5, 5, 
        ]}/>
        どれ？
      </div>
    </div>
    <p>
      1つだけそろっているならパターン1！<br/>
      どこもそろっていなければパターン2！<br/>
      全部がそろっていれば運が良い！！<br/>
    </p>
    <div style="display: grid; grid-template-columns: repeat(3, 1fr);">
      <div style="text-align: center">
      パターン1
      <Face colors={[
        6, 6, 6, 6, 6, 6, 6, 6, 6,

        7, 0, 0,
        0, 0, 0,
        0, 0, 0,
        0, 0, 7, 
      ]} classes={["vertical location2 size3  arrow1"]}/>
      →パターン1, 3<br/>
      </div>
      <div style="text-align: center">
        パターン2
        <Face colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
  
          0, 0, 0,
          0, 0, 0,
          0, 0, 0,
          0, 0, 0, 
        ]} classes={["vertical location2 size3  arrow1"]}/>
        →パターン1<br/>
      </div>
      <div style="text-align: center">
        パターン3
        <Face colors={[
          6, 6, 6, 6, 6, 6, 6, 6, 6,
  
          7, 0, 7,
          7, 0, 7,
          7, 0, 7,
          7, 0, 7, 
        ]}/>
        完成<br/>
      </div>
    </div>
    <h2>回し方</h2>
    <h3>1種類の回し方を覚える！</h3>
    <p>
      最後は緑面を正面にしてもつ！
    </p>
    <p>
      そろっているコーナーキューブを左上になるように持つことがポイント！<br/>
      そろっているキューブが無い場合はどこを左上にしても良いよ！
    </p>
    <p>完成するまで1～3回かかる！毎回向きをしっかり合わせよう！</p>
    <div style="display: grid; grid-template-columns: repeat(5, 1fr);">
      <div>
        <Step colors={[
          5, 5, 5, 5, 5, 5, 5, 5, 2,
    
          6, 6, 6, 6, 6, 6, 6, 6, 6, 
    
          3, 2, 2, 2, 2, 2, 3, 2, 2, 
        ]} notation="R2"/>
      </div>
      <div class="arrow">
        <Step colors={[
          5, 5, 4, 5, 5, 3, 5, 5, 3,
    
          6, 6, 1, 6, 6, 1, 6, 6, 1, 
    
          2, 2, 3, 2, 2, 2, 2, 2, 3, 
        ]} notation="D2"/>
      </div>
      <div class="arrow">
        <Step colors={[
          5, 5, 4, 5, 5, 3, 5, 5, 3,
    
          6, 6, 1, 6, 6, 1, 6, 1, 1, 
    
          2, 2, 3, 2, 2, 2, 4, 4, 2, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          5, 5, 6, 5, 5, 6, 5, 5, 6,
    
          6, 6, 4, 6, 6, 3, 6, 1, 3, 

          3, 2, 2, 2, 2, 4, 2, 2, 4, 
        ]} notation="U'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 6, 5, 5, 5, 5, 5, 5,
    
          4, 4, 4, 6, 6, 3, 6, 1, 3, 

          6, 6, 4, 2, 2, 4, 2, 2, 4, 
        ]} notation="R"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 4, 5, 5, 3, 5, 5, 3,
    
          4, 4, 1, 6, 6, 1, 6, 1, 1, 

          2, 2, 6, 2, 2, 6, 4, 4, 4, 
        ]} notation="D2"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 4, 5, 5, 3, 5, 5, 3,
    
          4, 4, 1, 6, 6, 1, 6, 6, 1, 
    
          2, 2, 6, 2, 2, 6, 2, 2, 3, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          6, 6, 6, 5, 5, 5, 5, 5, 5,
    
          4, 4, 4, 6, 6, 3, 6, 6, 3, 
    
          6, 6, 3, 2, 2, 2, 2, 2, 2, 
        ]} notation="U"/>
      </div>
      <div class="arrow">
        <Step colors={[
          5, 5, 6, 5, 5, 6, 5, 5, 6,
    
          6, 6, 3, 6, 6, 3, 6, 6, 3, 
    
          2, 2, 2, 2, 2, 2, 2, 2, 2, 
        ]} notation="R'"/>
      </div>
      <div class="arrow">
        <Step colors={[
          5, 5, 5, 5, 5, 5, 5, 5, 5, 

          6, 6, 6, 6, 6, 6, 6, 6, 6,

          2, 2, 2, 2, 2, 2, 2, 2, 2, 
        ]}/>
      </div>        
    </div>
    {/if}
  </div>
  <div id="param8">
    <h1 on:click={(e) => {show = show === 8 ? -1 : 8;}}><a href="#param8">8. 完成できたら</a></h1>
    {#if show === 8}
    <p>何回も繰り返しそろえて、何も見なくてもできるようになろう！</p>
    <p>このサイトで覚えた回し方は10通りくらいだけど、本格的にやるなら最低200通りくらい覚えることになる！</p>
    <p>回し方が上手になればこのやり方だけでも1分は切れるようになるはず！</p>
    <p>目指せ1分切り！！</p>
    <p><a href="https://www.pazru.net/LBL/">スピードキューブ攻略法</p>
    {/if}
  </div>
</main>

<style lang="scss">
  main {
    height: 100%;
  }
  h1
  {
    cursor: pointer;
    &:hover
    {
      text-decoration:underline;
    }
    > a
    {
      color:inherit;
      text-decoration: none;
    }
  }
  
</style>
