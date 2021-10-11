### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true 
### @explicitHints 1

# Beams of Color

## Step 1
�ǂɂ���F�t���u���b�N�Ɠ����F���ɂȂ�悤�ɁA�F�t���K���X��u�����B  
  
**�u���b�N�̐���:**  
``||ww:Move [forward] by (0)||`` �����_�[�E�[�}�����w�肵���u���b�N�� ��������B  
�@�@���@forward=�O�@back=���@left=���@right=�E  
``||ww:Turn [��]||`` �����_�[�E�[�}���̌�����ς���B  
``||ww:Place [Yellow] Stained Glass [forward]||`` �����_�[�E�[�}���ɃK���X��u������B  
�@�@���@Yellow=���F�@Lime=���C���@Blue=�@Red=��  

#### ~ tutorialhint 
```blocks
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.RedStainedGlass, Direction.Left)
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.LimeStainedGlass, Direction.Left)
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.BlueStainedGlass, Direction.Left)
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.YellowStainedGlass, Direction.Left)
})

```
```ghost
player.onChat("run", function () {
    for (let index = 0; index < 4; index++) {
        ww.moveWW(Direction.Forward, 1)
        ww.turnWW(LEFT_TURN)
        ww.placeBlock(BeamsGlass.YellowStainedGlass, Direction.Forward)
    }
})
```
```template
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.LimeStainedGlass, Direction.Right)
})
```
```package
minecraft-ww1984=github:tech8989/test/ww1984-ts
```