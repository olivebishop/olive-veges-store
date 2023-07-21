<template>
    <section class="home-products">

        <article class="shoe black">
            <RouterLink to="/product">
                <img src="@/assets/images/black1.png" alt="black-sneakers" id="product3" class="product">
                <h4>Black</h4>
                <figure>
                    <p>$200</p>
                    <img src="@/assets/images/cart.png" alt="cart">
                </figure>
            </RouterLink>
        </article>

        <article class="shoe brown">
            <RouterLink to="/product">
                <img src="@/assets/images/brown1.png" alt="black-sneakers" id="product3" class="product">
                <h4>Brown</h4>
                <figure>
                    <p>$200</p>
                    <img src="@/assets/images/cart.png" alt="cart">
                </figure>
            </RouterLink>
        </article>

        <article class="shoe white">
            <RouterLink to="/product">
                <img src="@/assets/images/white1.png" alt="black-sneakers" id="product3" class="product">
                <h4>White</h4>
                <figure>
                    <p>$200</p>
                    <img src="@/assets/images/cart.png" alt="cart">
                </figure>
            </RouterLink>
        </article>

    </section>
</template>

<script>
import '@/assets/styles/HomeProducts.scss';

export default {
    name: 'HomeProducts'
}
</script>