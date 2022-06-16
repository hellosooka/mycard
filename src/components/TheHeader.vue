<template>

<header>
    <div class="header__container">

        <!-- Табы -->
        <div class="tab">

            <input type="radio" name="radio2" value="3" id="tab-1" checked/>
            <label for="tab-1" class= "tab__1"> <p>Описание</p> </label>

            <input type="radio" name="radio2" value="4" id="tab-2" />
            <label for="tab-2" class= "tab__2"> <p>Услуги</p></label>

            <input type="radio" name="radio2" value="5" id="tab-3" />
            <label for="tab-3" class= "tab__3"> <p>Архив работ</p></label>

            <input type="radio" name="radio2" value="5" id="tab-4" />
            <label for="tab-4" class= "tab__4"> <p>Технологии</p></label>

            <input type="radio" name="radio2" value="5" id="tab-5" />
            <label for="tab-5" class= "tab__5"> <p>Контакты</p></label>

            <div class="tab__color"></div>
        </div>
        <div class="header__title">
            Земцов Леонид
        </div>
    </div>

</header>

</template>

<script>
export default {

}
</script>

<style lang="scss">
:root {
    --primary-light: #8ab9ff;
    --primary: #5d97fc;
    --primary-dark: #0e6aeb;

    --white: #FFFFFF;
    --greyLight-1: #E4EBF5;
    --greyLight-2: #c8d0e7;
    --greyLight-3: #bec8e4;
    --greyDark: #9baacf;
}

$shadow: .3rem .3rem .6rem var(--greyLight-2),
-.2rem -.2rem .5rem var(--white);
$inner-shadow: inset .2rem .2rem .5rem var(--greyLight-2),
inset -.2rem -.2rem .5rem var(--white);

.header__title {
    position: absolute;
    top: 40px;
    left: 50px;

    font-size: 75px;
    font-weight: bold;

    @media(max-width: 1600px) {
        position: relative;
    }

}

.tab {

    margin: 40px 45px 20px auto;
    grid-column: 3 / 4;
    grid-row: 1 / 2;
    width: 54rem;
    height: 4rem;
    box-shadow: $shadow;
    border-radius: 1rem;
    display: flex;
    align-items: center;

    @media(max-width: 950px) {
            margin: 20px auto;
            flex-direction: column;
            height: 27rem;
            width: 93%;
            grid-column: 0;

    }

    input { display: none; }

    > input:checked + label {
    transition: all .5s ease;
    color: var(--primary);
    }

    &__1, &__2, &__3, &__4, &__5 {
        width: 30.8rem;
        height: 4.6rem;
        font-size: 1.4rem;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        color: var(--greyDark);
        transition: all .5s ease;

        @media(max-width: 950px) {
            margin: 20px auto;
            font-size: 2.4rem;

        }

        &:hover { color: var(--primary); }

    }

    &__color {
        position: absolute;
        height: 3.4rem;
        width: 10.2rem;
        margin-left: .3rem;
        border-radius: .8rem;
        box-shadow: $inner-shadow;
        pointer-events: none;

        @media(max-width: 950px) {
            margin: 0.7rem;
            width: 90%;
            height: 3.6rem;

        }
    }
}

#tab-1:checked ~ .tab__color {
    transform: translateX(0);
    transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    @media(max-width: 950px) {
            transform: translateY(0);
            transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    }

}
#tab-2:checked ~ .tab__color {
    transform: translateX(10.7rem);
    transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    @media(max-width: 950px) {
            transform: translateY(5.5rem);
            transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    }
}
#tab-3:checked ~ .tab__color {
    transform: translateX(21.4rem);
    transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    @media(max-width: 950px) {
            transform: translateY(11rem);
            transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    }
}
#tab-4:checked ~ .tab__color {
    transform: translateX(32.4rem);
    transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    @media(max-width: 950px) {
            transform: translateY(16.2rem);
            transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    }
}
#tab-5:checked ~ .tab__color {
    transform: translateX(43.1rem);
    transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    @media(max-width: 950px) {
            transform: translateY(21.8rem);
            transition: transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);

    }
}

</style>
