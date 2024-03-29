# Archived
Due to short time and complexity to write the entire code from BCAPP, I've decided to [rewrite in Java.](https://github.com/gotneb/bcapp-api) 

# BCAPP
 A BCAPP's api library written in Go.
 ## :milky_way: API
 
 All of them return in a JSON format.
 
 ### :bookmark: ECC's endpoints
 
<details><summary>modp</summary><p>
 
It has the same parameters meaning from Ecc.modp(BigInteger n, BigInteger p1). [See java file.](https://github.com/carlosamcruz/BCAPP/blob/master/app/src/main/java/com/nibblelinx/BCAPP/Ecc.java#L47)
 
#### HTTP Request

```
GET https://bcapp-go.herokuapp.com/modp/<n>/<p1>
```
 #### URL Parameters

| Parameter  |  Description  |
| --- | --- |
|  n |  Big Integer |
|  p1 |  Big Integer |

</p>

</details>

<details><summary>inverse</summary><p>
 
It has the same parameters meaning from Ecc.inverse(BigInteger r, BigInteger p). [See java file.](https://github.com/carlosamcruz/BCAPP/blob/master/app/src/main/java/com/nibblelinx/BCAPP/Ecc.java#L54)
 
#### HTTP Request

```
GET https://bcapp-go.herokuapp.com/inverse/<r>/<p>
```
 #### URL Parameters

| Parameter  |  Description  |
| --- | --- |
|  r |  Big Integer |
|  p |  Big Integer |

</p>

</details>

<details><summary>doublep</summary><p>
 
It has the same parameters meaning from Ecc.doublep(BigInteger x, BigInteger y). [See java file.](https://github.com/carlosamcruz/BCAPP/blob/master/app/src/main/java/com/nibblelinx/BCAPP/Ecc.java#L81)
 
#### HTTP Request

```
GET https://bcapp-go.herokuapp.com/doublep/<x>/<y>
```
 #### URL Parameters

| Parameter  |  Description  |
| --- | --- |
|  x |  Big Integer |
|  y |  Big Integer |

</p>

</details>

<details><summary>addp</summary><p>
 
It has the same parameters meaning from Ecc.addp(BigInteger x1, BigInteger y1, BigInteger x2, BigInteger y2). [See java file.](https://github.com/carlosamcruz/BCAPP/blob/master/app/src/main/java/com/nibblelinx/BCAPP/Ecc.java#L96)
 
#### HTTP Request

```
GET https://bcapp-go.herokuapp.com/addp/<x1>/<y1>/<x2>/<y2>
```
 #### URL Parameters

| Parameter  |  Description  |
| --- | --- |
|  x1 |  Big Integer |
|  y1 |  Big Integer |
|  x2 |  Big Integer |
|  y2 |  Big Integer |

</p>

</details>

<details><summary>eccnp</summary><p>
 
It has the same parameters meaning from Ecc.eccnP(BigInteger n, BigInteger x, BigInteger y). [See java file.](https://github.com/carlosamcruz/BCAPP/blob/master/app/src/main/java/com/nibblelinx/BCAPP/Ecc.java#L128)
 
#### HTTP Request

```
GET https://bcapp-go.herokuapp.com/eccnp/<n>/<x>/<y>
```
 #### URL Parameters

| Parameter  |  Description  |
| --- | --- |
|  n |  Big Integer |
|  x |  Big Integer |
|  y |  Big Integer |

</p>

</details>
 
## :memo: Test Driven
Check-out the [source files](https://github.com/gotneb/bcapp/tree/main/files_tests) :file_folder: used in the tests.
 - [x] modp
 - [x] inverse
 - [ ] doublep
 - [ ] addp
 - [ ] eccnp
