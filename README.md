![IMG_20251117_141859](https://github.com/user-attachments/assets/5d5a56f0-a0a8-4334-b9e3-2c4ba3fab680)![IMG_20251117_142608](https://github.com/user-attachments/assets/b34f1133-67ba-4870-ad92-31fb92f4c20e)# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
![IMG_20251117_141859](https://github.com/user-attachments/assets/a11fc97c-b0dc-458d-a9e9-c72312bdd06f)
![IMG_20251117_141949](https://github.com/user-attachments/assets/ef4d2d3d-7990-45f0-93e3-1f27d161271c)







## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
```
num=[1]
den=[1 15 50 0]
sys=tf(num,den)
rlocus(sys)
[k poles]=rlocfind(sys)
```

## Output:
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/cb425b4f-2be1-496b-8d5f-faf7ac5618b4" />

```
num =

     1


den =

     1    15    50     0


sys =
 
           1
  -------------------
  s^3 + 15 s^2 + 50 s
 
Continuous-time transfer function.
Model Properties
Select a point in the graphics window

selected_point =

  -0.0611 + 7.1575i


k =

  762.3762


poles =

 -15.0448 + 0.0000i
   0.0224 + 7.1185i
   0.0224 - 7.1185i
```


## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is 762.3762
