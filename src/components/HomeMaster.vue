<template>
<div>
        <vue-snotify></vue-snotify>
<v-container grid-list-md mb-0>
  <v-row justify="space-around">
    <v-col cols="5" class="mt-12">
       <h1 class="display-3 font-weight-black text-center mt-12" style="color: #DEB887">Data Master</h1>   
    </v-col>
    <v-col cols="5">
        <v-row justify="space-around">
        <v-col cols="2" class="mt-12">
          <v-tooltip bottom>
            <template v-slot:activator="{ on }">
                
            <v-avatar color="#FFE4C4" size="62" class="mb-5">
                <v-btn icon link to="datahewan">
                  <v-icon v-on="on" > mdi-48px mdi-cow</v-icon>
                  </v-btn>
            </v-avatar>
                
            </template>
              <span>Hewan</span>
            </v-tooltip>
            
            
            <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#D2B48C" size="62" class="mb-5">
                 <v-btn icon link to="supplier">
                  <v-icon v-on="on"> mdi-48px mdi-cube-outline</v-icon>
                 </v-btn>
            </v-avatar>
            </template>
              <span>Supplier</span>
            </v-tooltip>
        </v-col>
        <v-col cols="2" class="mt-12">
           <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#FFF8DC" size="62" class="mb-5">
                 <v-btn icon link to="ukuranHewan">
                  <v-icon v-on="on"> mdi-48px mdi-ruler</v-icon>
                 </v-btn>
            </v-avatar>
            </template>
              <span>Ukuran hewan</span>
            </v-tooltip>
            
            <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#FFDAB9" size="62" class="mb-5">
                <v-btn icon link to="layanan">
                  <v-icon v-on="on"> mdi-48px mdi-ambulance</v-icon>
                </v-btn>
            </v-avatar>
            </template>
              <span>Layanan</span>
            </v-tooltip>
        </v-col>
        <v-col cols="2" class="mt-12">
           <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#F5DEB3" size="62" class="mb-5">
                <v-btn icon link to="jenisHewan">
                  <v-icon v-on="on"> mdi-48px mdi-paw</v-icon>
                </v-btn>
            </v-avatar>
            </template>
              <span>Jenis Hewan</span>
            </v-tooltip>
            
           <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="brown" size="62" class="mb-5">
                <v-btn icon link to="produk">
                  <v-icon v-on="on"> mdi-48px mdi-food-variant</v-icon>
                </v-btn>
            </v-avatar>
            </template>
              <span>Produk</span>
            </v-tooltip>
        </v-col>
        <v-col cols="2" class="mt-12">
           <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#DEB887" size="62" class="mb-5">
                <v-btn icon link to="dataCustomer">
                  <v-icon v-on="on"> mdi-48px mdi-human-male-female</v-icon>
                </v-btn>
            </v-avatar>
            </template>
              <span>Customer</span>
            </v-tooltip>
            
            <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#FFDEAD" size="62" class="mb-5">
                <v-btn icon link to="pegawai">
                  <v-icon v-on="on"> mdi-48px mdi-account-key</v-icon>
                </v-btn>
            </v-avatar>
            </template>
              <span>Pegawai</span>
            </v-tooltip>
        </v-col>
        </v-row>
    </v-col>
  </v-row>
  <v-divider class="ml-12 mr-12"></v-divider>
  <v-row justify="space-around">
    <v-col cols="4">
        <v-row justify="space-around">
        <v-col cols="2" class="mt-9">
          <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#FAEBD7" size="62" class="mb-5">
                <v-btn icon link to="daftarStokHabis">
                  <v-icon v-on="on"> mdi-48px mdi-minus-box-outline</v-icon>
                </v-btn>
            </v-avatar>
            </template>
              <span>Stok Habis</span>
            </v-tooltip>
        </v-col>
        <v-col cols="2" class="mt-9">
          <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#FFFACD" size="62" class="mb-5">
                <v-btn icon link to="addPengadaan">
                  <v-icon v-on="on"> mdi-48px mdi-cart-plus</v-icon>
                </v-btn>
            </v-avatar>
            </template>
              <span>Tambah Pengadaan</span>
            </v-tooltip>
        </v-col>
        <v-col cols="2" class="mt-9">
          <v-tooltip bottom>
            <template v-slot:activator="{ on }">
            <v-avatar color="#FFE4B5" size="62" class="mb-5">
                <v-btn icon link to="layoutHistory">
                  <v-icon v-on="on"> mdi-48px mdi-history</v-icon>
                </v-btn>
            </v-avatar>
            </template>
              <span>History</span>
            </v-tooltip>
        </v-col>
        </v-row>
    </v-col>
    <v-col cols="5">
        <h1 class="display-3 font-weight-black text-center mt-12" style="color: #DEB887">Pengadaan Produk</h1>   
    </v-col>
  </v-row>

  <v-divider class="ml-12 mr-12 mt-12"></v-divider>
  <v-row justify="space-around">
    <v-col cols="5" class="mt-12">
        <h1 class="display-3 font-weight-black text-center mt-12" style="color: #DEB887">Laporan Toko</h1> 
    </v-col>
    <v-col cols="5">
          <v-row justify="space-around">
        <v-col cols="2" class="mt-12">
          <v-tooltip bottom>
            <template v-slot:activator="{ on }">
              <v-badge
                color="red"
                content="Bulanan"
                overlap
              >
            <v-avatar color="brown lighten-5" size="62" class="mb-5">
                <v-btn icon link to="pendapatanBulanan">
                  <v-icon v-on="on"> mdi-48px mdi-decimal-increase</v-icon>
                </v-btn>
            </v-avatar>
              </v-badge>
            </template>
              <span>Pendapatan Bulanan</span>
            </v-tooltip>
            
            
            <v-tooltip bottom>
            <template v-slot:activator="{ on }">
              <v-badge
                color="red"
                content="Tahunan"
                overlap
              >
            <v-avatar color="#D2B48C" size="62" class="mb-5">
                <v-btn icon link to="pendapatanTahunan">
                  <v-icon v-on="on"> mdi-48px mdi-decimal-increase</v-icon>
                </v-btn>
            </v-avatar>
              </v-badge>
            </template>
              <span>Pendapatan Tahunan</span>
            </v-tooltip>
        </v-col>
        <v-col cols="2" class="mt-12">
           <v-tooltip bottom>
            <template v-slot:activator="{ on }">
              <v-badge
                color="red"
                content="Bulanan"
                overlap
              >
            <v-avatar color="#FFF8DC" size="62" class="mb-5">
                <v-btn icon link to="pengadaanBulanan">
                  <v-icon v-on="on"> mdi-48px mdi-cube-send</v-icon>
                </v-btn>
            </v-avatar>
              </v-badge>
            </template>
              <span>Pengadaan Bulanan</span>
            </v-tooltip>
            
            <v-tooltip bottom>
            <template v-slot:activator="{ on }">
              <v-badge
                color="red"
                content="Tahunan"
                overlap
              >
            <v-avatar color="#FFDAB9" size="62" class="mb-5">
                <v-btn icon link to="pengadaanTahunan">
                  <v-icon v-on="on"> mdi-48px mdi-cube-send</v-icon>
                </v-btn>
            </v-avatar>
              </v-badge>
            </template>
              <span>Pengadaan Tahunan</span>
            </v-tooltip>
        </v-col>
        <v-col cols="2" class="mt-12">
           <v-tooltip bottom>
            <template v-slot:activator="{ on }">
              <v-badge
                bordered
                color="error"
                icon="mdi-star-outline"
                overlap
                
              >
            <v-avatar color="brown lighten-2" size="62" class="mb-5">
                <v-btn icon link to="produkTerlaris">
                  <v-icon v-on="on">mdi-48px mdi-food-variant</v-icon>
                </v-btn>
            </v-avatar>
              </v-badge>
            </template>
            
              <span>Produk Terlaris</span>
            </v-tooltip>
            
           <v-tooltip bottom>
            <template v-slot:activator="{ on }">
              <v-badge
                bordered
                color="error"
                icon="mdi-star-outline"
                overlap
                
              >
            <v-avatar color="brown lighten-3" size="62" class="mb-5">
                <v-btn icon link to="layananTerlaris">
                  <v-icon v-on="on"> mdi-48px mdi-ambulance</v-icon>
                </v-btn>
            </v-avatar>
              </v-badge>
            </template>
              <span>Layanan Terlaris</span>
            </v-tooltip>
        </v-col>
        </v-row>
    </v-col>
  </v-row>
</v-container>
</div>
</template>
<script>
import Snotify from 'vue-snotify';
  export default {
    data () {
      return {
          show1: false,
          show2: false,
          show3: false,
          produk: [],
      }
    },
    methods:{
        getDataStok(){
            var uri = this.$apiUrl + '/produk/stokHabis'
            this.$http.get(uri).then( (response) =>{
                this.produk=response.data
                console.log(this.produk.length)
                if(this.produk.length>"0"){
                this.$snotify.confirm('Beberapa Stok produk Habis', 'Cek Sekarang!', {
                timeout: 1000,
                showProgressBar: true,
                closeOnClick: false,
                pauseOnHover: true,
                buttons: [
                    {text: 'Cek Produk', action: (toast) => {console.log('Clicked: Later'); this.$router.push({ name: "daftarStokHabis" });} },
                    {text: 'Close', action: (toast) => {console.log('Clicked: No'); this.$snotify.remove(toast.id); }, bold: true},
                ]
                });
            }
            })
        },
    },
    mounted(){
    this.getDataStok();
    if (localStorage.getItem("token") != null) {
        if(localStorage.getItem("peran")=="Kasir"){
              window.location.replace('/homeKasir')
        }else if(localStorage.getItem("peran")=="Customer Service"){
              window.location.replace('/homeCS')
        }else if(localStorage.getItem("peran")=="Owner"){
              next()
        }
    }
    else{
      window.location.replace('/home')
    }
    }
  }
</script>