<template>
  <div>

    <center>
      <div class="text-center text-4xl text-green-500 pt-20 w-1/3 border-b border-gray-400">
        Staff
      </div>
    </center>

    <div class="flex flex-wrap">

      <div class="flex flex-wrap w-full py-12 justify-center">
        <img class="bild" src="https://www.linkpicture.com/q/Erling.png">
        <div class="w-1/4 pl-80">
          <div class="text-xl text-green-500">Erling Blomberg</div>
          <div class="flex flex-wrap text-lg">Programmerare</div>
        </div>
      </div>

      <div class="flex flex-wrap w-full py-12 justify-center">
        <img class="bild"
          src="data:image/jpeg;base64,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">
        <div class="w-1/4 pl-80">
          <div class="text-xl text-green-500">Victor Vatn</div>
          <div class="flex flex-wrap text-lg">Programmerare</div>
        </div>
      </div>

      <div class="flex flex-wrap w-full pt-12 justify-center">
        <img class="bild" src="https://www.linkpicture.com/q/jag_2.png">
        <div class="w-1/4 pl-80">
          <div class="text-xl text-green-500">Tim Sjöstrand</div>
          <div class="flex flex-wrap text-lg">Programmerare</div>
        </div>
      </div>
    </div>

    <div>
      <center>
        <div class="text-center text-4xl text-green-500 pt-20 w-1/3 border-b border-gray-400">
          About Ruby Zebras
        </div>
      </center>
      <div class="text-center py-12 text-lg">
        Pancakes with cream
      </div>
    </div>

  </div>
</template>

<script>
export default {

}
</script>

<style>
.bild {
  border-radius: 50%;
  width: 150px;
  height: 150px;
}

/*
.bilder {
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  justify-content: flex-start;
  align-items: baseline;
  align-content: stretch;
  margin-left: 100px;

}

.rad {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-items: center;
  align-content: stretch;
  margin-bottom: 30px;
}

.namn {
  margin-left: 10%;
  font-size: 50px;
  width: 500px;
} */
</style>
