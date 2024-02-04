<template>
    <h2>Nutrition</h2>
    <p>The table below shows nutritional values per serving whithout the additional fillings.</p>
    <table>
        <tr>
            <td>Calories</td>
            <td>277kcal</td>
        </tr>
        <tr>
            <td>Carbs</td>
            <td>0g</td>
        </tr>
        <tr>
            <td>Protein</td>
            <td>20g</td>
        </tr>
        <tr>
            <td>Fat</td>
            <td>22g</td>
        </tr>
    </table>
</template>

<style scoped>
    p{
        font-size: .9em;
        font-weight:400;
        font-family:'Outfit';
        color:hsl(24, 5%, 18%);
    }
    tr{
        width: 100%;
        display: flex;
        justify-content: safe;
        gap: 110px;
        padding-left:20px;
        padding-bottom:10px;
        margin-bottom:10px;
        border-bottom: 1px solid hsl(30, 18%, 87%);
    }
    td{
        width: 100px;
        overflow:hidden;
        color:hsl(24, 5%, 18%);
        font-weight:500;
    }
    td:nth-child(2){
        color: hsl(14, 45%, 36%);
        font-weight:700;
    }
</style>