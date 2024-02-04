<script setup>
    import omelette from '@/assets/img/image-omelette.jpeg'
    import Ingredients from '@/components/recipe/Ingredients.vue'
    import Instructions from '@/components/recipe/Instructions.vue'
    import Nutrition from '@/components/recipe/Nutrition.vue'
</script>

<template>
    <div class="card">
        <img :src="omelette" alt="omelette" class="card-img-top">
        <div class="card-body">
            <div class="card-title">Simple Omelette Recipe</div>
            <p class="card-text">An easy and quick dish, perfect for any meal. This classic omelette is made with beaten eggs cooked to perfection, optionally filled with your choice of cheese, vegetables, or meats.</p>
            <hr>
            <div class="card-preparation">
                <h3>Preparation time</h3>
                <ul>
                    <li><span>Total:</span> Appoximately 10 minutes</li>
                    <li><span>Preparation:</span> 5 minutes</li>
                    <li><span>Cooking:</span> 5 minutes</li>
                </ul>
            </div>
            <Ingredients/>
            <hr>
            <Instructions/>
            <hr>
            <Nutrition/>
        </div>

    </div>
</template>

<style>
    .card{
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        border-radius: 20px;
    }
    .card-img-top{
        width: 90%;
        object-fit: cover;
        margin: 30px;
        border-radius: 10px;
    }
    .card-body{
        width: 90%;
        height: auto;
        display: flex;
        flex-direction: column;
        margin: auto;
    }
    .card-title{
        font-size: 1.7em;
        font-weight: 400;
        font-family: 'Young Serif';
        color: hsl(24, 5%, 18%);
    }
    .card-text{
        font-size: .98em;
        font-weight: 400;
        font-family: 'Outfit';
        line-height: 1.4em;
        color: hsl(24, 5%, 18%);

    }
    .card-preparation{
        width: 90%;
        margin: auto;
        margin-left: 30px;
        background-color: hsl(330, 100%, 98%);
        padding: 10px 20px;
    }
    .card-preparation h3{
        color: hsl(332, 51%, 32%);
        font-weight: 600;
        font-family: 'Outfit';
    }
    .card-preparation ul{
        list-style: none;
        padding-left: 0;
    }
    li{
        position: relative;
        padding-left: 30px; 
        margin-bottom: 7px;
        font-family: 'Outfit';
        color:hsl(30, 10%, 34%);
        font-weight: 400;
    }
    .card-preparation ul li::before{
        content: '\25A0';
        color: hsl(24, 5%, 18%);
        font-size: 7px;
        position: absolute;
        top: 1px;
        left: 0;
    }
    li span{
        color: hsl(30, 10%, 34%);
        font-family: 'Outfit';
        font-weight: 600;
    }
    hr{
        width: 100%;
        height: 1px;
        background: hsl(30, 18%, 87%);
        border: none;
    }

    @media (width <=768px){
        .card-img-top{
            width: 100%;
            margin: 0px;
            border-radius: 10px;
        }  
        .card-body{
            width: 85%;
        }
        .card-title{
            font-size: 2.2em;
        }
        .card-preparation{
            width: 90%;
            margin: auto;
            margin-left: 10px;
            background-color: hsl(330, 100%, 98%);
            padding: 10px;
        }
    }
</style>