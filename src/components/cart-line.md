```jsx
let lines = [
   {_id: 'Keyboard',
    title: 'Keyboard',
    imageUrl: "https://images.unsplash.com/photo-1560769629-975ec94e6a86?ixid=MnwyNDY1NjJ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2MjYyNDYyMDc&ixlib=rb-1.2.1&auto=format&fit=crop&w=543&h=384&q=80&&ixlib=rb-1.2.1&&auto=format&&fit=crop&&w=40&&h=40&&q=80",
    price: 204,
    quantity: 1,
    amount: 204,
   },
   {_id: 'Table',
    title: 'Table',
    imageUrl: "https://images.unsplash.com/photo-1553456558-aff63285bdd1?ixid=MnwyNDY1NjJ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2MjYyNDYyMDc&ixlib=rb-1.2.1&auto=format&fit=crop&w=543&h=384&q=80&&ixlib=rb-1.2.1&&auto=format&&fit=crop&&w=40&&h=40&&q=80",
    price: 709,
    quantity: 1,
    amount: 709,
   },
   {_id: 'Ball',
    title: 'Ball',
    imageUrl: "https://images.unsplash.com/photo-1525966222134-fcfa99b8ae77?ixid=MnwyNDY1NjJ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2MjYyNDYyMDc&ixlib=rb-1.2.1&auto=format&fit=crop&w=543&h=384&q=80&&ixlib=rb-1.2.1&&auto=format&&fit=crop&&w=40&&h=40&&q=80",
    price: 92,
    quantity: 2,
    amount: 184,
   },
];

const deleLine = (pid) => {alert(`Line item for ${pid} will be removed.`)}

import CartLine from "./cart-line"; 
    <ul id="cart-item-list" className="divide-y divide-gray-200">
        {lines && lines.map(line => (
            <CartLine
               key={line._id}
               title={line.title}
               imageUrl={line.imageUrl}
               price={line.price}
               quantity={line.quantity}
               amount={line.amount}
               onDele={() => deleLine(line._id)}
        />
        ))}
    </ul>
```