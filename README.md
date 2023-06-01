# implementandoFormularios
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aprendendo sobre formulários</title>
</head>
<body>    
    <!--Usando formulários (tag <form>)-->
        <!--"Action" é utilizado para apontar onde os dados vão ser enviados-->
        <form name="signup" onsubmit="alert('Seus dados foram enviados')" autocomplete="on" method="post" action="https://meusite.com.br/signup">
            <h2>Tag "form"</h2>
            Nome: <input type="text" name="name"/><br>
            Idade: <input type="number" name="age"/><br>
            Senha: <input type="password" name="password"/><br>
            <button type="submit">Enviar</button>
            <hr>
        </form>

     <!--Usando "input"-->
     <h2>Usando input</h2>
     <label>Test:</label><input type="text"/><br>
     <label>Number:</label><input type="number" min="0" step="5" max="99"/><br>
     <label>Button:</label><input type="button" value="Enviar"/><br>
     <label>Range:</label><input type="range"/><br>
     <label>Color:</label><input type="color"/><br>
     <label>Email:</label><input type="email"/><br>
     <label>URL</label><input type="url"/><br>
     <label>Date:</label><input type="date"/><br>
     <label>Week:</label><input type="week"/><br>
     <label>Month:</label><input type="month"/><br>
     <label>Checkbox:</label><input type="checkbox"/><br>
     <label>Radio:</label><input type="radio" name="aceita"/><br>
     <label>Button:</label><input type="button" value="Enviar"/><br>
     <label>Hidden:</label><input type="hidden" name="Hidden"><br>
     <label>File: </label><input type="file"><br>
     <label>Search: </label><input type="search"><br>

     <!--Se aprofundando no checkbox e radio-->
     <hr>
     <h2>Formulário de cliente</h2>
     <form method="post">
        <h3>Você selecionou: Pizza de Calabresa</h3>
        <p>Quais opcionais você deseja</p>
        <input type="checkbox" name="opcional[]" value="queijo"> + queijo <br> 
        <input type="checkbox" name="opcional[]" value="calabresa"> + calabresa <br>
        <input type="checkbox" name="opcional[]" value="cebola"> + cebola <br>
        <input type="checkbox" name="opcional[]" value="azeitona"> + azeitona <br>
        <p>Borda recheada?</p>
        <input type="radio" name="Borda" value="sim"> Sim <br>
        <input type="radio" name="Borda" value="nao"> Não <br>
        <p>Bebida</p>
        <input type="radio" name="Bebida" value="suco"> Suco <br>
        <input type="radio" name="Bebida" value="Refrigerante"> Refrigerante <br>
        <input type="radio" name="Bebida" value="agua"> Água <br>
        <input type="radio" name="Bebida" value="nenhum"> Nenhum <br>
        <p></p>
        <button type="submit">Enviar pedido</button><br><p></p>
        <hr>

        <!--Button e Seus Tipos-->

        <form onsubmit="get">
            <h2>Button e seus tipos</h2>
            <label>Nome </label><input type="text" name="name"><br>
            <label>Idade </label><input type="number" name="age"><br>
            <label>Password </label><input type="password" name="password"><br><p></p>
            <button type="button">Clicável</button><br>
            <button type="reset">Limpar</button><br>
            <button type="submit">Enviar</button> <!--no "submit" tem que prestar atenção em validar as informações. Se valida colocando "onsubmit" sentro da TAG "form"-->
        </form>
        <hr>

        <!--Select e Seus Tipos-->

        <form onsubmit="" method="get"><h2>Método Select</h2>
            <label>Nome:</label><input type="text" name="name"><br>
            <label>Cargo:</label>
            <select name="role">
                <option value="">Selecione o cargo</option>
                <option value="Administrativo">Administrativo</option>
                <option value="Gerente">Gerente</option>
                <option value="diretor">Diretor</option>
                <option value="presidente">Presidente</option>                
            </select><br>
            <button type="submit">Enviar</button>        
        </form>
        <hr>

        <!--Textarea-->

        <form onsubmit="get"><h2>Textarea</h2>
            <label>Mensagem:</label><br>
            <textarea name="message" id="" cols="30" rows="10"></textarea><br>
            <button type="submit">Enviar</button>        
        </form>            

     </form>
</body>
</html>
