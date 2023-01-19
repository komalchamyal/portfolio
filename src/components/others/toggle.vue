<template>

    <div>
        <input type="checkbox" v-model="isActive" @click="toggle" class="checkbox" id="checkbox">
        <label for="checkbox" class="checkbox-label">
            <i class="fas fa-moon"></i>
            <i class="fas fa-sun"></i>
            <span class="ball"></span>
        </label>
    </div>
    {{ isActive }}

</template>

<script>
export default {
    name: 'toggle-mode',
    data() {
        return{
        isActive: true
        }
    },
    methods:
    {
        toggle() {
            this.isActive = this.isActive ? false : true;
        },
    }
}
</script>

<style>

body.dark {
    background-color: #292c35;
}

/* #9b59b6 */

body.dark h1,
body.dark a {
    color: #fff;
}

.checkbox {
    opacity: 0;
    position: absolute;
}

.checkbox-label {
    background-color: #111;
    width: 50px;
    height: 26px;
    border-radius: 50px;
    position: relative;
    padding: 5px;
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.fa-moon {
    color: #f1c40f;
}

.fa-sun {
    color: #f39c12;
}

.checkbox-label .ball {
    background-color: #fff;
    width: 22px;
    height: 22px;
    position: absolute;
    left: 2px;
    top: 2px;
    border-radius: 50%;
    transition: transform 0.2s linear;
}

.checkbox:checked+.checkbox-label .ball {
    transform: translateX(24px);
}
</style>