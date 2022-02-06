# HTML-HW3

3 разных типа полей расположить на странице, сделать валидацию (проверку заполняемости) поля, одного или нескольких в одной форме. 
<form>   
     <input type=" " >
    <input type=" " required>
    <input type=" " >
    <input type="submit" >
    <input type="reset" >
</form>

1. Забыли фигурную скобку в стилях
2. В последней форме нет <input type="submit"> и <input type="reset">
---------------------------------------------------------------------


<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Document</title>
	<style type="text/css">
		
table , tr, td ,th {
	width: 1200px;
	
	background: dimgray;
	border:  1.5px solid black;
	 color: white;
	 font-size: 19px;
 









	</style>
</head>
<body>
<table >

	<tr>
		<th>Элемент Формы</th>
		<th>Верификация</th>
		<th>Валидация</th>
	</tr>

	<tr>
		<td><span style="color: red;">Submit</span> форма отправки</td>
		<td>заполнить форму и нажать на кнопку Отправить</td>
		<td>
			<form>
				<input type="text" value="">
				<input type="submit" >
				<input type="Reset" value="Сброс" >
				
			</form>
		</td>	
	</tr>

	<tr>
		<td><span style="color: red;">Reset</span> форма сброса</td>
		<td>После ввода текста,при активациии кнопки происходит сброс данных</td>
		<td>
			<form>
				<input type="text" placeholder="ввести текст">
				<input type="submit" >
				<input type="Reset" value="Сброс" >
			</form>
		</td>
	</tr>
		<td>
			<span style="color: red;">List</span> выпадающее меню</td>
		<td>в приведенном меню выбрать опцию , и нажать отправить<td>
			<form>	
  				<input type="text" list="view testing" placeholder="указать вид">
					<datalist id="view testing">
						<option>value="Модульное"</option>
						<option>value="Системное"</option>
						<option>value="Сквозное"</option>
  					</datalist>
  				<input type="submit" value="Отправить">
  				<input type="Reset" value="Сброс" >
  			</form>
  	<tr>	
  		<td>
  			<span style="color: red;">Password</span> пароль безопасности</td>
  		<td>ввести пароль до 8 символов</td>
  		<td><form>
  				<input type="password" placeholder="ввести пароль" name="asdasd" maxlength="8">
  				<input type="submit" value="Подтвердить">
  				<input type="Reset" value="Сброс" >
  			</form>
  		</td>
  	</tr>

  	<tr>
  		<td>
  			<span style="color: red;">Range</span> Регулятор выбора </td>
  		<td>
  			<form>
  				<label for="volume">проверить ползунок,подвигать лево право</label><td>
  				<input type="range" id="volume" name="volume" min="0" max="5">
  			</form>
  		</td>
  	</tr>	
  						
  					
 </table>



	
</body>
</html>
