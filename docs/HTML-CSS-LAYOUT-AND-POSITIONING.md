# HTML & CSS - Layout and Positioning  

---

## 📌 Index:    

1. **[Flex🔻](#default-properties-of-flex-container)** 
2. **[🧭 Position🔻](#position)** 

---   

## Flex   

```css
#container {
  /* Item from left to right on the main axis and top to bottom on the cross axis */
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  /* Shorthand for flex-direction and flex-wrap */
  flex-flow: row nowrap;
  /* Aligns items along the cross axis */
  align-items: center;
  /* Aligns items along the main axis */
  justify-content: space-between;
}
```

> [!NOTE]
> **For flex-wrap to work, the container or its children must have a size constraint**

```css
.container {
  display: flex;
  flex-wrap: wrap;
  /* Limits width to trigger wrapping */
  width: 300px; 
}

.item {
  /* Items will wrap when they exceed container width */
  flex-basis: 150px; 
}
```



**[🔝 Back to Top](#html--css---layout-and-positioning)**

---  

## Position  



```css

```



**[🔝 Back to Top](#html--css---layout-and-positioning)**

---