# Revue de code de Noa-Pelletier

## Points positifs

- Le code est **bien structuré**, ce qui facilite la lecture et la maintenance.
- Il semble avoir été **développé sans IA**, ce qui montre une bonne compréhension des concepts.
- **Bonne utilisation des Watch**, permettant une gestion efficace des changements d'état.

```js
watch(
  () => props.product,
  (newProduct) => {
    if (newProduct) {
      modifiedProductName.value = newProduct.title
      modifiedProductDescription.value = newProduct.description
      modifiedProductColor.value = newProduct.color
      modifiedProductStock.value = newProduct.stock
      modifiedProductPrice.value = newProduct.price
    }
  },
  { immediate: true }
)
```

## Points negatif

- CSS et scripts ne sont pas dans les dossiers
- Précense de **HelloWorld**
- Pas de validation de form pour éviter la _duplication_
- Les forms n'utilisent pas bootstrap
