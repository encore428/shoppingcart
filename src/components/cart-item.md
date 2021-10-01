```jsx
  const prods = [
    { _id: "Bike",
      title: "Bike",
      price: 938,
      description: "Juice Drink Concept",
      condition: "new",
      availability: "single-item",
      imageUrl: "https://images.unsplash.com/photo-1570831739435-6601aa3fa4fb?ixid=MnwyNDY1NjJ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2MjYyNDYyMDc&ixlib=rb-1.2.1&fit=crop&w=543&h=384&q=80",
      canAdd: true
    },
    { _id: "Ball",
      title: "Ball",
      price: 690,
      description: "Black vintage Seiko leather watch",
      condition: "new",
      availability: "single-item",
      imageUrl: "https://images.unsplash.com/photo-1596460107916-430662021049?ixid=MnwyNDY1NjJ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2MjYyNDYyMDc&amp;ixlib=rb-1.2.1&auto=format&fit=crop&w=543&h=384&q=80",
      canAdd: true
    },
    { _id: "Tuna",
      title: "Tuna",
      price: 999,
      description: "NIKE FREE",
      condition: "new",
      availability: "in-stock",
      numOfStock: 2,
      imageUrl: "https://images.unsplash.com/photo-1542291026-7eec264c27ff?ixid=MnwyNDY1NjJ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2MjYyNDYyMDc&ixlib=rb-1.2.1&auto=format&fit=crop&w=543&h=384&q=80",
      canAdd: true
    }
];

const add2Cart = (pid) => {alert(`Product ${pid} will be added to Cart.`)}
  <div className="bg-gray-50 lg:flex">
    <div className="flex-1">
      <div className="max-w-7xl mx-auto pt-16 pb-24 px-4 sm:px-6 lg:px-8">
        <div className="grid md:grid-cols-2 gap-x-4 gap-y-8 xl:grid-cols-3 xl:gap-x-6">
          {prods.map(prod => (
            <CartItem 
                key={prod._id}
                title={prod.title}
                price={prod.price}
                description={prod.description}
                condition={prod.condition}
                availability={prod.availability}
                numOfStock={prod.numOfStock}
                imageUrl={prod.imageUrl}
                authed={prod.canAdd}
                onAdd={() => add2Cart(prod._id)}
            />
          ))}
        </div>
      </div>
    </div>
  </div>
```
