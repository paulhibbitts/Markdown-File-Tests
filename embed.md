## Test area for embedded content

Here's the result:

<div style="width: 400px; height: 300px;">
  <lume-scene webgl>
    <lume-box id="box" size="100 100 100" mount-point="0.5 0.5 0.5" color="royalblue" rotation="10 20 30"></lume-box>
    <lume-camera-rig initial-distance="500" min-distance="100" max-distance="1200">
      <lume-point-light color="white" position="-500 -500 500"></lume-point-light>
    </lume-camera-rig>
  </lume-scene>
</div>
<style>
  lume-scene { border: 1px solid deeppink; }
</style>

<script>
  async function loadScript(URL) {
    const response = await fetch(URL)
    const code = await response.text()
    const script = document.createElement('script')
    script.textContent = code
    document.head.append(script)
  }
  loadScript('https://unpkg.com/lume@0.3.0-alpha.26/dist/global.js').then(() => {
    const {defineElements} = LUME
    defineElements() // defines the Lume elements
    const box = document.getElementById('box') // get a reference to the <lume-box> element
    box.rotation = (x, y, z) => [x, y+0.2, z+0.2] // make it rotate
  })
</script>

<script type="text/javascript" src="https://ssl.gstatic.com/trends_nrtr/3349_RC01/embed_loader.js"></script> <script type="text/javascript"> trends.embed.renderExploreWidget("TIMESERIES", {"comparisonItem":[{"keyword":"smallrig","geo":"US","time":"today 5-y"}],"category":0,"property":""}, {"exploreQuery":"date=today%205-y&geo=US&q=smallrig&hl=en","guestPath":"https://trends.google.com:443/trends/embed/"}); </script>

Above shown google trends for "smallrig."
