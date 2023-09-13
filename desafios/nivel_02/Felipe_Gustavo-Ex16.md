## Olá pelo visto consegui
Segue código abaixo:
## Código Php
~~~php
//Esse trecho vai dentro da div com id 'php'

<?php
    if (!empty($_POST)) {
        for ($i = 1; $i < 11; $i++) {
            echo $_POST["vezes"]." X ".$i." = ".$_POST["vezes"]*$i."<br>";
        };
    };
?>
~~~
## Código HTML
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>EX-16</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-4bw+/aepP/YC94hEpVNVgiZdgIC5+VKNBQNGCHeKRQN+PtmoHDEXuppvnDJzQIu9" crossorigin="anonymous">
</head>

<body>
    <div class="container">
        <h1>Multiplicação</h1>
        <form action="" method="POST">
            <div class="mb-3">
                <label for="multiplicador" class="form-label">Coloque o numero que você quer multiplicar:</label>
                <input type="number" class="form-control" id="vezes" name="vezes">
                <button type="submit" class="btn btn-success">Enviar</button>
        </form>
    </div>
    <div class="container" id="php">
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-HwwvtgBNo3bZJJLYd8oVXjrBZt8cqVSpeBNS5n7C8IVInixGAoxmnlMuBnhbgrkm" crossorigin="anonymous"></script>
</body>

</html>
~~~
