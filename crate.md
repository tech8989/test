### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true 
### @explicitHints 1

# Suspicious Crates

## Step 1
��������̖ؔ��̊Ԃ�ʂ��āA�ʂ��܂ꂽ�G��̈ꕔ���Ȃ������ׂ悤�B  
�G�悪��������A���̔������킵�āA��ɓ���悤�B  
  
�����͉��p�^�[��������̂ŁA�����ȃp�^�[�����l���Ă݂悤�B  
  
**�u���b�N�̐���:**  
``||ww:Move [forward] by (0)||`` �����_�[�E�[�}�����w�肵���u���b�N�� ��������B  
�@�@���@forward=�O�@back=���@left=���@right=�E  
``||ww:Turn [��]||`` �����_�[�E�[�}���̌�����ς���B  
``||ww:painting inside crate [forward]||`` �ؔ��̒��ɊG�悪�Ȃ����𒲂ׂ�B  
``||ww:Break crate [forward]||`` �ؔ����󂷁B


```ghost
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
    if (ww.locatePainting(Direction.Forward)) {
        ww.retrievePainting(Direction.Forward)
    }
    for (let index = 0; index < 4; index++) {
        
    }
    while (!(false)) {
        
    }	
})
```
```template
player.onChat("run", function () {
    if (ww.locatePainting(Direction.Forward)) {

    }
})
```
```package
minecraft-wwheist=github:tech8989/wwheist
```