Setting up React.

```diff
- text in red
+ text in green
! text in orange
# text in gray
```

```diff
# Using ES5 Syntax
-   this.state.products.forEach(function(product){
-      ProductViews.push(<Product productInfo={product} key={product.id} onUpdateProductWithId={this.updateProductWithId} />)
-   }.bind(this))
- 


# Using ES6 Syntax - Arrow functions
# Notice how we got rid of function, return, bind(this) keywords
+ this.state.products.forEach(product=>{
+      ProductViews.push(
+         <Product
+           productInfo={product}
+          key={product.id}
+          onUpdateProductWithId={this.updateProductWithId}
+         />
+       );
+      }
+    );
    
 ```
