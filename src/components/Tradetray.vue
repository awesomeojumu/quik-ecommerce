<template>
        <div class="col-lg-4 col-md-6 mb-4">
            <div class="card h-90 my-4">
                <img class="card-img-top" 
                      :src="product.imageLink" 
                      :alt="product.name" 
                      height="200" 
                >
                <div class="card-body">
                    <div>
                        <h5 class="card-title">
                            <a href="#">{{product.name}}</a>
                        </h5>
                    </div>
                    <div>
                        <h6> &#8358;{{product.price}}</h6>
                    </div>
                    <button class="btn btn-primary btn-sm">Buy Now</button>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name: 'Tradetray',
    props: ['product']
}
</script>

<style scoped>
.card:hover {
  box-shadow: 8px 12px 31px -10px #ab98ab;
}
.card:hover .card-body .card-title {
  margin-bottom: .5rem;
}
.card-height{
  height: auto;
}
</style>