<template>
    <div class="filter">
        <div class="category-filter">
            <div :class="`category-${i}`" v-for="i in 4" :key="i" tabindex="0">
                <div class="filter-back"></div>
                <p :class="`category-${i}-name`"> {{ categoryArr[i-1] }} </p>
                <p :class="`category-${i}-amount`"> 3 </p>
            </div>

        </div>

        <div class="slider-filter">
            <div class="category-header">
                <p class="price"> Цена </p>
            </div>
            <div class="frame-1066">
                <div class="price-from">
                    <p class="price-from-txt"> от </p>
                    <input class="price-from-input" type="text" placeholder="5500 ₽"/>
                </div>
                <img class="divider" src="/common/other/divider.svg" alt="divider">
                <div class="price-to">
                    <p class="price-to-txt"> до </p>
                    <input class="price-to-input" type="text" placeholder="5500 ₽"/>
                </div>
            </div>
        </div>

        <div class="checkbox-filter-1">
            <div class="checkbox-filter-1-category-header">
                <p class="checkbox-filter-1-brand-txt"> Бренд </p>
                <p class="checkbox-filter-1-clear-txt"> Очистить </p>
            </div>
            <div class="checkbox-filter-1-search-input-wrapper">
                <div class="frame-1059">
                    <img class="checkbox-filter-1-search-icon" src="/common/other/search.svg">
                    <input class="checkbox-filter-1-search-input" type="text" placeholder="Поиск.."/>
                </div>
            </div>
            <div class="frame-1152">
                <div class="frame-1152-checkbox-wrapper" v-for="i in 10" :key="i">
                    <div class="frame-1049">
                        <input class="frame-1049-checkbox" type="checkbox"/>
                        <p class="frame-1049-checkbox-name"> Атрибут </p>
                    </div>
                    <p class="frame-1152-amount"> 333 </p>
                </div>
            </div>
        </div>

        <div class="checkbox-filter-2">
            <div class="checkbox-filter-2-category-header">
                <p class="checkbox-filter-2-brand-txt"> Размер </p>
            </div>
            <div class="frame-1252">
                <div class="frame-1252-checkbox-wrapper" v-for="i in 10" :key="i">
                    <div class="frame-1149">
                        <input class="frame-1149-checkbox" type="checkbox"/>
                        <p class="frame-1149-checkbox-name"> Атрибут </p>
                    </div>
                    <p class="frame-1252-amount"> 333 </p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            categoryArr: new Array(4).fill("Название категории")
        }
    }
}
</script>