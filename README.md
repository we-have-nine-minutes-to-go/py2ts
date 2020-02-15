# py2ts
A transpiler python to typescript

## Goal of 2020
sample.py
```python
class ShoppingList(Component):
    def render(self):
        return f'''
            <div className="shopping-list">
              <h1>Shopping List for {self.props.name}</h1>
              <ul>
                <li>Instagram</li>
                <li>WhatsApp</li>
                <li>Oculus</li>
             </ul>
           </div>
        '''
```
result.tsx
```typescript
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}
```
