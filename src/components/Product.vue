<template>
    <div class="container">
        <!-- <div class="card">
            <div class="container-product">
                <div class="letak-gambar"></div>
                <div class="letak-deskripsi">
                    <div class="letak-deskripsi-top"></div>
                    <div class="letak-deskripsi-bottom"></div>
                </div>
            </div>
        </div> -->
        <div class="container">
            <div class="background">
                <img src="../assets/bg-pattern.svg" alt="background">
            </div>
            <div class="card">
                <!-- <div class="container-unavailable-product">
                    <div class="background">
                        <img src="../assets/sad-face.svg" alt="sad">
                    </div>
                    <div class="product-details">
                        <p>This product is unavailable to show</p>
                        <div class="tombol">
                            <button type="button" class="tombol-next">Next Product</button>
                        </div>
                    </div>
                </div> -->
                <div class="container-product">
                    <div class="image-product">
                        <img src="" alt="">
                    </div>
                    <div class="product-details">
                        <div class="top">
                            <h3 class="title">Men Casual Slim Fit</h3>
                            <div class="sub-title">
                                <div class="rate">
                                    <p>men clothing</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Product',
    data() {
        return {
            
        }
    },
    methods: {
        async API(){
            const response = await fetch('https://fakestoreapi.com/products');
            const result = await response.json();
            return result;
        }
    },
}
</script>
<style scoped>
    @import '../css/style.css'
</style>