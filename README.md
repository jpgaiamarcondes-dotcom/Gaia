# Lorentz Calculator

Calculadora estática e interativa para explorar boosts de Lorentz e testar invariantes numéricos. Não requer dependências ou etapa de build.

## Usar

Abra `index.html` em um navegador. Informe os componentes de β = v/c e selecione **Gerar matriz**. A calculadora usa a métrica de Minkowski η = diag(1, −1, −1, −1) e a convenção ct′ = γ(ct − β·x).

A matriz Λ pode ser editada diretamente. **Verificar invariantes** calcula ΛᵀηΛ e compara cada elemento com η, mostrando o erro absoluto máximo e det(Λ). A seção de quadrivetor compara s² = (ct)² − x² − y² − z² antes e depois de X′ = ΛX. A tolerância ajustável trata erros de arredondamento de ponto flutuante.

## Escopo

- Boosts em 3 dimensões espaciais, com |β| < 1.
- Verificação numérica da condição de Lorentz ΛᵀηΛ = η.
- Verificação do intervalo de Minkowski para um quadrivetor fornecido.
- Sem bibliotecas externas; cálculos em JavaScript usando números IEEE 754.
