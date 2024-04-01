<template>
    <div>
        <div class="bodi">
            <div class="left">
                <h2>Informasi Pribadi</h2>
                <p><strong>Nama: </strong>Taufik Mahaldi</p>
                <p><strong>Umur: </strong>20</p>
                <p><strong>Email: </strong>taufikmahaldi059@gmail.com</p>
                <h2>Sosial Media</h2>
                <ul>
                    <li v-for="sosmed in sosialMedia" :key="sosmed.id">
                        {{ sosmed.platform }}<a :href="`https://${sosmed.url}`" target="_blank" rel="noopener noreferrer">{{ sosmed.username }}</a>
                    </li>
                </ul>

                <h2>Hobi</h2>
                <ul>
                    <li>Membaca</li>
                    <li>Main Game</li>
                    <li>Ngoding</li>
                </ul>
            </div>
            <div class="right">
                <h2>About Me</h2>
                <p>Saya adalah seorang mahasiswa Teknik Informatika di Universitas Islam Riau.</p>
                <h2>Pendidikan</h2>
                <h3>Teknik Informatika 2022 - Now</h3>
                <p>Universitas Islam Riau</p>
                <h3>Teknik Komputer dan Jaringan 2019 - 2022</h3>
                <p>SMKN 2 Pekanbaru</p>
                <h2>Pengalaman</h2>
                <h3>Magang di PT.WanXP (April 2021 - September 2021)</h3>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'BodyCV',
}
</script>

<script setup>
const sosialMedia = [
    { id: 1, platform: 'Instagram: ', username: '@taufik.maha', url: 'www.instagram.com/taufik.maha' },
    { id: 2, platform: 'Youtube: ', username: '@taufikmahaldi1003', url: 'www.youtube.com/@taufikmahaldi1003'},
    { id: 3, platform: 'Facebook: ', username: 'Taufik Mahaldi', url: 'www.facebook.com/taufik.mahaldi'}
]
</script>

<style scoped>
.bodi{
    display: flex;
    flex-wrap: wrap;
}
.left{
    flex: 1;
    padding: 30px;
}
.left p{
    line-height: 2;
}
.left ul li{
    line-height: 2;
}
h2{
    background: #00b6c4;
    padding: 15px;
    color: #fff;
    margin: 30px 0;
    font-size: 20px;
    border-radius: 0 50px 50px 0;
}
h3{
    font-weight: 500px;
}
.right{
    flex: 1;
    padding: 30px;
}
.right h3{
    margin-bottom: 15px;
}
.right p{
    line-height: 2.9;
}
.right ul li{
    line-height: 2;
}
</style>