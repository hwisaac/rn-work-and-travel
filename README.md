# Work and Travel

투두리스트

- input
- button
- state
- data persistance


## 컴포넌트
### [TouchableOpacity](https://reactnative.dev/docs/touchableopacity) 
> 이 컴포넌트로 감싸면 클릭할 때 투명도를 줍니다.

### [TouchableHighlight](https://reactnative.dev/docs/touchablehighlight)
> 요소를 클릭하면 배경색을 바꿔줍니다.

### [TouchableWithoutFeedback](https://reactnative.dev/docs/touchablewithoutfeedback)

- one child 만 넣어야 합니다. 여러 컴포넌트를 넣고싶다면 `View` 로 감싸야 합니다.

```js
function MyComponent(props: MyComponentProps) {
  return (
    <View {...props} style={{flex: 1, backgroundColor: '#fff'}}>
      <Text>My Component</Text>
    </View>
  );
}

<TouchableWithoutFeedback onPress={() => alert('Pressed!')}>
  <MyComponent />
</TouchableWithoutFeedback>;
```
### [TextInput](https://reactnative.dev/docs/textinput)
> 텍스트 인풋 컴포넌트 <br />
> 이 컴포넌트를 누르면 키보드가 뜬다.

```js
const [working, setWorking] = useState(true);
const [text, setText] = useState('');

<TextInput
  onChangeText={onChangeText}
  value={text}
  placeholder={ 'Add a To Do' }
  style={styles.input}
/>
```

![](readMeImages/2023-07-06-13-03-29.png)