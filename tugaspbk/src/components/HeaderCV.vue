<template>
    <div >
        <div class="heder">
            <div class="imgarea">
                <img src="../assets/foto.jpeg" alt="foto saya">
            </div>
            <h1>Taufik Mahaldi</h1>
            <h3>Mahasiswa Teknik Informatika</h3>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HeaderCV',
}
</script>

<style scoped>

.heder{
    text-align: center;
}
.heder h1{
    margin-bottom: 10px;
}
.heder h3{
    text-transform: uppercase;
    font-size: 15px;
    font-weight: 500;
}
.imgarea{
    width: 200px;
    height: 200px;
    border-radius: 50%;
    overflow: hidden;
    margin: 25px auto;
    border: 15px groove deepskyblue;
}
.imgarea img{
    width: 100%;
}
</style>