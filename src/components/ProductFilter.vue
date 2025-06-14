<template>
    <div class="filter">
        <div class="category-filter">
            <div class="category-1"> 
                <p class="category-1-name"> Название категории </p>
                <p class="category-1-amount"> 3 </p>
            </div>
            <div class="category-2"> 
                <p class="category-2-name"> Название категории </p>
                <p class="category-2-amount"> 3 </p>
            </div>
            <div class="category-3"> 
                <p class="category-3-name"> Название категории </p>
                <p class="category-3-amount"> 3 </p>
            </div>
            <div class="category-4"> 
                <p class="category-4-name"> Название категории </p>
                <p class="category-4-amount"> 3 </p>
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