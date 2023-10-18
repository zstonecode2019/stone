# stone
a mvvm lib for three d scene display

# component
import { useState } from 'stone';
export default function Box() {
  const [color, setColor] = useState("#00ff00");
  
  const onChangeColor = () => {
    setColor('#ff0000');
  }
  
  return (
    <mesh geometry={type: 'box', width: 1, height: 1, depth: 1} material={{type: 'basic', color}} @click={onChangeColor}></mesh>
  )
}
