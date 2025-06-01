<script setup>

</script>

<template>
    <div class="container">
        <h1>Calculadora Aritmética</h1>
        <div class="input-group">
            <input type="number" placeholder="Digite o primeiro número"/>
            <input type="number" placeholder="Digite o segundo número"/>
        </div>

        <select name="" class="select">
            <option value="+">Soma (+)</option>
            <option value="-">Subtração (−)</option>
            <option value="*">Multiplicação (×)</option>
            <option value="/">Divisão (÷)</option>
        </select>

        <div class="resultado">
            <p>Resultado</p>
            <h2>{{  }}</h2>
        </div>
    </div>
</template>

<style scoped>
    .container {
        max-width: 400px;
        margin: 0 auto;
        padding: 2rem 1rem;
        display: flex;
        flex-direction: column;
        align-items: stretch;
        gap: 1rem;
        background: linear-gradient(to bottom right, #4f46e5, #3b82f6);
        color: white;
        border-radius: 12px;
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        font-family: 'Poppins', sans-serif;
    }

    h1 {
        text-align: center;
        font-size: 1.8rem;
        margin-bottom: 0.5rem;
    }

    .input-group {
        display: flex;
        flex-direction: column;
        gap: 0.8rem;
    }

    input,
    select {
        padding: 0.8rem;
        font-size: 1.1rem;
        border-radius: 8px;
        border: none;
        outline: none;
    }

    input:focus,
    select:focus {
        box-shadow: 0 0 0 3px rgba(255, 255, 255, 0.3);
    }

    .select {
        background: white;
        color: #1f2937;
    }

    .resultado {
        text-align: center;
        background: rgba(255, 255, 255, 0.15);
        padding: 1rem;
        border-radius: 10px;
    }

    .resultado h2 {
        font-size: 2rem;
        margin-top: 0.5rem;
    }
</style>
