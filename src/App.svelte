<script lang="ts">
  import svelteLogo from "./assets/svelte.svg";
  import viteLogo from "/vite.svg";
  import Cube from "./lib/Cube.svelte";
  import Step from "./lib/Step.svelte";
  import Face from "./lib/Face.svelte";
</script>

<main>
  <div>
    <h1>0. キューブの基本</h1>
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
    <p>どれだけ回転させても、この3つのキューブの位置は変わらない。</p>
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
    <div style="display: grid; grid-template-columns: repeat(2, 1fr;">
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

  </div>
  <div>
    <h1>1. クロスをそろえる</h1>
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
      ]}/>
    </div>
  <div >
    <Step colors={[
      0, 1, 0, 1, 1, 0, 0, 1, 0,

      0, 2, 0, 0, 2, 1, 0, 0, 0,

      0, 0, 0, 3, 3, 0, 0, 0, 0,
    ]} notation="U'"/>
  </div>

  </div>
  <h3>2段目に無い場合は1度回す！</h3>
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
    <div >
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
  <div>
    <h1>2. 一面をそろえる</h1>
    <Step colors={[
      1, 1, 1, 1, 1, 1, 1, 1, 1,

      2, 2, 2, 0, 2, 0, 0, 0, 0,

      3, 3, 3, 0, 3, 0, 0, 0, 0,
    ]}/>
    <p>入れたい位置の真下に持ってくることがポイント！</p>
    <h2>回し方</h2>
    <h3>2種類の入れ方を覚える！</h3>
    <p>真下に持ってきたコーナーキューブの青面を自分にむけると、この2つのどちかになる！</p>
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
    <p>次の手順を行い、向きを変えてあげる必要がある。</p>
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
    <p>適当なキューブを入れてあげよう。</p>
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
  </div>
  <div>
    <h1>3. 2列目をそろえる</h1>
  </div>
  
  <div>
    <h1>4. 上面のクロスをそろえる</h1>
  </div>
  <div>
    <h1>5. 上面の色をそろえる</h1>
  </div>
  <div>
    <h1>6. エッジキューブの向きをそろえる</h1>
  </div>
  <div>
    <h1>7. コーナーキューブの向きをそろえる</h1>
  </div>
</main>

<style>
  main {
    height: 100%;
  }
  
</style>
