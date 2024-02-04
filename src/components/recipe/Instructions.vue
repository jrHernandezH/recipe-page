<template>
    <h2>Instructions</h2>
    <ol>
        <li v-for="instruction in dataInstructions" :key="instruction.id" class="instruction-item">
            <span class="instruction-number">{{ instruction.id }}.</span>
            <div class="text-instruction">
                <span>{{ instruction.title }}:</span>
                {{ instruction.text }}
            </div>
        </li>
    </ol>
</template>

<script setup>
    const dataInstructions = [
        {
            id: 1,
            title: 'Beat the eggs',
            text: 'In a bowl, beat the eggs with a pinch of salt and pepper until they are well mixed. You can add a tablespoon of water or milk for a fluffier texture.'
        },
        {
            id: 2,
            title: 'Heat the pan',
            text: 'Place a non-stick frying pan over medium heat and add butter or oil.'
        },
        {
            id: 3,
            title: 'Cook the omelette',
            text: 'Once the butter is melted and bubbling, pour in the eggs. Tilt the pan to ensure the eggs evenly coat the surface.'
        },
        {
            id: 4,
            title: 'Add fillings (optional)',
            text: 'When the eggs begin to set at the edges but are still slightly runny in the middle, sprinkle your chosen fillings over one half of the omelette.'
        },
        {
            id: 5,
            title: 'Fold and serve',
            text: 'As the omelette continues to cook, carefully lift one edge and fold it over the fillings. Let it cook for another minute, then slide it onto a plate.'
        },
        {
            id: 6,
            title: 'Enjoy',
            text: 'Serve hot, with additional salt and pepper if needed.'
        }
    ];
</script>

<style scoped>
    ol {
        list-style: none;
        padding-left: 0;
    }
    ol li{
        display:flex;
        margin-bottom:20px;
    }

    .instruction-number {
        color: hsl(332, 51%, 32%);
        font-size: 12px;
        margin-right: 15px;
    }
    .text-instruction{
        color:hsl(30, 10%, 34%);
    }

</style>
