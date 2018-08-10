<template>
    <div class="centered">
        <a href="https://discordapp.com/api/oauth2/authorize?client_id=412139349770108939&permissions=372632694&scope=bot">
            <img class="rounded-circle dborder bbpic" src="../assets/images/bb.png" />
        </a>
        <img class="rounded-circle status" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAQAAAC0NkA6AAAALElEQVR42u3NMQEAAAwCoNm/9DL4eEEBcgORSCQSiUQikUgkEolEIpFIJJ0HCt8AM0IRFnUAAAAASUVORK5CYII=">
    </div>
</template>

<script>
export default {
  name: 'BearFloat'
}
</script>

<style lang="sass" scoped>
$border: #2c2f33;
$dnd: #ee4747;

.centered
  left: 50%;
  margin-left: -100px;
  margin-top: -50px;
  position: fixed;
  top: 50%;

.dborder
  animation: float 7s ease-in-out infinite;
  border: 4px solid $border;
  height: 200px;
  position: static;
  width: 200px;

.status
  animation: float 7s ease-in-out infinite;
  background-color: $dnd;
  border: 4px solid $border;
  height: 35px;
  margin-top: -90px;
  position: absolute;
  right: 5px;
  top: 245px;

.rounded-circle
  border-radius: 50%;


// https://codepen.io/MarioDesigns/pen/woJgeo

@keyframes float
  0%
    box-shadow: 0 5px 15px 0 rgba(0, 0, 0, .6);
    transform: translatey(0);

  50%
    box-shadow: 0 25px 15px 0 rgba(0, 0, 0, .2);
    transform: translatey(-20px);

  100%
    box-shadow: 0 5px 15px 0 rgba(0, -1, 0, .6);
    transform: translatey(0);
</style>

