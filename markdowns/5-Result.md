#### EXAMPLE 5)

#### AC:
Counts the duplicate value inside an array


```javascript
const inventory = ['popsicle', 'underwear', 'sauce', 'pens', 'potatoes', 'sauce', 'onion', 'onion', 'pens', 'potatoes', 'ukulele', 'tomahawk', 'underwear', 'popsicle', 'sauce', 'ukulele', 'onion', 'underwear', 'popsicle', 'potatoes', 'onion', 'pens', 'ukulele'];

const countItems = inventory => {
    return inventory.reduce((acc, name) => ({
        …acc,
        [name]: acc[name] ? acc[name] + 1 : 1
    }), {});
};
countItems(inventory); //  { onion: 4, pens: 3,popsicle: 3,potatoes: 3,sauce: 3,tomahawk: 1,ukulele: 3,underwear: 3 }
```
