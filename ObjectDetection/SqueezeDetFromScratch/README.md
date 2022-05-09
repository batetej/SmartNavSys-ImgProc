<h1 align="center"> Implementación de SqueezeDet (C y Python) </h1> 

## Resultados Zybo


Nombre de la capa | Salida     | filter	size/stride | S1x1 | e1x1 | e3x3 | C Time[s] | Py Time[s] 
------------------| ---------- | ------------------ | ---- | ---- | ---- | ------    | ------- 
Input             | 320x240x3  | ---------------    | ---- | ---- | ---- | 0.04228   | ------- 
Conv1             | 160x120x64 | 3x3/2	(x64)       | ---- | ---- | ---- | 0.741     | ------- 
maxpool1          | 80x60x64   | 3x3/2              | ---- | ---- | ---- | 0.06      | -------
fire2	          | 80x60x128  | ---------------    | 16   | 64   | 64	 | 0.6481    | -------
fire3	          | 80x60x128  | ---------------    | 16   | 64   | 64   | 0.85      | -------
maxpool3          | 154x46x128 | 3x3/2              | ---- | ---- | ---- | 0.03      | -------
fire4	          | 154x46x256 | ---------------    | 32   | 128  | 128  | 0.64      | -------
fire5	          | 154x46x256 | ---------------    | 32   | 128  | 128	 | 0.83      | -------
maxpool5          | 76x22x256  | 3x3/2              | ---- | ---- | ---- | 0.01      | -------	
fire6	          | 76x22x384  | ---------------    | 48    | 192 | 192  | 0.37      | ------- 
fire7	          | 76x22x384  | ---------------    | 48    | 192 | 192  | 0.41      | -------	
fire8	          | 76x22x512  | ---------------    | 64    | 256 | 256  | 0.68      | -------	
fire9	          | 76x22x512  | ---------------    | 64    | 256 | 256  | 0.76      | -------
fire10	          | 76x22x768  | ---------------    | 96    | 384 | 384  | 1.57      | -------
fire11	          | 76x22x768  | ---------------    | 96    | 384 | 384  | 1.81      | -------
ConvDet           | 76x22x72   | 3x3/1	(x72)       | ---- | ---- | ---- | 3.85      | -------
Output            | ---------- | ---------------    | ---- | ---- | ---- | 13.3      | -------