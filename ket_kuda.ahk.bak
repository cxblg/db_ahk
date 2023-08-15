; #Include <FindText>
#SingleInstance, force
; #Include <FindText>
WinGetPos, posKX, posKY,,,A
;WinGetPos, posKX, posKY,,,ahk_class Sandbox:2cc4:TForm1
t1:=A_TickCount, X:=Y:=""

Text:="|<>*174$32.0000000000200860U0200D3tkNu9W86nW0W1g8VsUNm9m867WEW1UMYMUPC8vA6S00000000000000000000000000000000000000000000V/U008HA0024V000V8E008G408"

koorScanX1 := posKX + 163, koorScanY1 := posKY + 53
koorScanX2 := posKX + 255, koorScanY2 := posKY + 391
if (ok:=FindText(X, Y, koorScanX1, koorScanY1, koorScanX2, koorScanY2, 0, 0, Text))
{
  ; FindText.Click(X, Y, "L")
}
kuda_posY := ""
if (Y = 83)
{
tooltip, "83", 5, 5
kuda_posY := 83
}
if (Y = 140)
{
tooltip, "140", 5, 5
kuda_posY := 140
}

; ok:=FindText("wait",3, 0,0,0,0,0,0,Text)    ; Wait 3 seconds for appear
; ok:=FindText("wait0",-1, 0,0,0,0,0,0,Text)  ; Wait indefinitely for disappear

;MsgBox, 4096, Tip, % "Found:`t" Round(ok.Length())
;  . "`n`nTime:`t" (A_TickCount-t1) " ms"
;  . "`n`nPos:`t" X ", " Y
;  . "`n`nResult:`t<" (Comment:=ok[1].id) ">"

for i,v in ok
  if (i<=2)
    FindText.MouseTip(ok[i].x, ok[i].y)

