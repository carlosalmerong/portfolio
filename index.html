<!DOCTYPE HTML>
<html>

<head>
	<style>
		.error {
			color: #FF0000;
		}

		#formulario {
			border-style: solid;
			padding: 20px;
			margin-right: 25%;
		}
	</style>
</head>

<body>
	<div id="formulario">
		<?php
		$errorNombre = $errorApellido = $errorSexo = $errorFecNac = $errorSueldo = $errorCategoria = $errorAficiones = "";
		$nombre = $apellidos = $sexo = $sueldo = $fechaNac = $categoria = $aficiones = $categoriaGuardada = "";

		$arrayNombres = array();
		$arrayApellidos = array();
		$arrayFecNacs = array();
		$arraySueldos = array();
		$arraySexos = array();

		if ($_SERVER["REQUEST_METHOD"] == "POST") {
			if (empty($_POST["nombre"])) { // Si esta vacío salta error
				$errorNombre = "Escribe un nombre";
				$nombre = "";
			} else {
				$nombre = formatear($_POST["nombre"]);
				// Revisa la integridad del texto
				if (!preg_match("/^[a-zA-Z- ]{3,}/", $nombre)) {
					$errorNombre = "Mínimo 3 caracteres y solo letras";
					$nombre = "";
				}
			}
		}

		if (empty($_POST["apellidos"])) {
			$errorApellido = "Introduce algún apellido por favor";
		} else {

			if (!preg_match("/^[a-zA-Z-' ]*$/", $apellidos)) {
				$errorApellido = "Solo se permiten letras y espacios en blanco";
			} else {
				$apellidos = formatear($_POST["apellidos"]);
				if (str_contains($apellidos, " ")) {
					$apellidos = formatear($_POST["apellidos"]);
				} else {
					$errorApellido = "Introduce dos apellidos, por favor";
					$apellidos = "";
				}
			}
		}

		if (empty($_POST["fechaNac"])) {
			$errorFecNac = "Introduce una fecha de nacimiento";
		} else {
			$fechaNac = formatear($_POST["fechaNac"]);
			if (!validarFecha($fechaNac)) {
				$errorFecNac = "Fecha de nacimiento inválida";
				$fechaNac = "";
			}
		}

		if ($_POST["categorias"] == "elige") {
			$errorCategoria = "Introduce una categoria";
		} else {
			$categoria = formatear($_POST["categorias"]);
		}

		if (empty($_POST["sueldo"])) {
			$errorSueldo = "Introduce un sueldo";
		} else {
			$sueldo = formatear($_POST["sueldo"]);
			if (!preg_match("/[0-9]/", $sueldo)) {
				$errorSueldo = "No se pueden introducir datos que no sean números";
				$sueldo = "";
			} else {
				if ($categoria == "peon") {
					if ($_POST["sueldo"] >= 600 && $_POST["sueldo"] <= 1200 && empty($errorSueldo)) {
						$sueldo = formatear($_POST["sueldo"]);
					} else {
						$errorSueldo = "Sueldo no válido, no está entre 600 y 1200";
						$sueldo = "";
					}
				} else if ($categoria == "oficial") {
					if ($_POST["sueldo"] >= 900 && $_POST["sueldo"] <= 1500 && empty($errorSueldo)) {
						$sueldo = formatear($_POST["sueldo"]);
					} else {
						$errorSueldo = "Sueldo no válido, no está entre 900 y 1500";
						$sueldo = "";
					}
				} else if ($categoria == "jefe") {
					if ($_POST["sueldo"] >= 1400 && $_POST["sueldo"] <= 2500 && empty($errorSueldo)) {
						$sueldo = formatear($_POST["sueldo"]);
					} else {
						$errorSueldo = "Sueldo no válido, no está entre 1400 y 2500";
						$sueldo = "";
					}
				} else if ($categoria == "director") {
					if ($_POST["sueldo"] >= 2000 && $_POST["sueldo"] <= 3000 && empty($errorSueldo)) {
						$sueldo = formatear($_POST["sueldo"]);
					} else {
						$errorSueldo = "Sueldo no válido, no está entre 2000 y 3000";
						$sueldo = "";
					}
				}
			}
		}

		if (empty($_POST["sexo"])) {
			$errorSexo = "Sexo requerido";
		} else {
			$sexo = formatear($_POST["sexo"]);
		}

		if (empty($_POST["deportes"]) && empty($_POST["lectura"]) && empty($_POST["musica"]) && empty($_POST["cine"]) && empty($_POST["idiomas"])) {
			$errorAficiones = "Selecciona una afición";
		} else {

			if (!empty($_POST["deportes"])) {
				$aficiones = $aficiones . " " . formatear($_POST["deportes"]);
			}
			if (!empty($_POST["lectura"])) {
				$aficiones = $aficiones . " " . formatear($_POST["lectura"]);
			}
			if (!empty($_POST["musica"])) {
				$aficiones = $aficiones . " " . formatear($_POST["musica"]);
			}
			if (!empty($_POST["cine"])) {
				$aficiones = $aficiones . " " . formatear($_POST["cine"]);
			}
			if (!empty($_POST["idiomas"])) {
				$aficiones = $aficiones . " " . formatear($_POST["idiomas"]);
			}

			if (trim($aficiones) == 'deportes' && $sexo == 'hombre') {
				$errorAficiones = "Un hombre debe tener más aficiones";
				$aficiones = "";
			}
		}


		function formatear($data)
		{
			$data = trim($data);
			$data = stripslashes($data);
			$data = htmlspecialchars($data);
			return $data;
		}

		function validarFecha($fecha, $format = "d/m/Y")
		{
			$d = DateTime::createFromFormat($format, $fecha);
			return $d && $d->format($format) == $fecha;
		}
		?>

		<h2>Alta Datos Empleado</h2>
		<p><span class="error">* campo requerido</span></p>
		<form method="post" action="<?php echo htmlspecialchars($_SERVER["PHP_SELF"]); ?>">
			Nombre: <input type="text" name="nombre" value="<?php echo $nombre; ?>">
			<span class="error">* <?php echo $errorNombre; ?></span>

			<br><br>

			Apellidos: <input type="text" name="apellidos" value="<?php echo $apellidos; ?>">
			<span class="error">* <?php echo $errorApellido; ?></span>

			<br><br>

			Fecha de nacimiento: <input type="text" name="fechaNac" value="<?php echo $fechaNac; ?>">
			<span class="error">* <?php echo $errorFecNac; ?></span>

			<br><br>

			Sueldo: <input type="text" name="sueldo" value="<?php echo $sueldo; ?>">
			<span class="error">* <?php echo $errorSueldo; ?></span>

			<br><br>

			Categoría:
			<select name="categorias">
				<option value="elige" selected="selected">Elige</option>
				<option value="peon">Peón</option>
				<option value="oficial">Oficial</option>
				<option value="jefe">Jefe Departamento</option>
				<option value="director">Director</option>
			</select>
			<span class="error">* <?php echo $errorCategoria; ?></span>

			<br><br>

			Sexo:
			<input type="radio" name="sexo" <?php if (isset($sexo) && $sexo == "mujer") echo "checked"; ?> value="mujer">Mujer
			<input type="radio" name="sexo" <?php if (isset($sexo) && $sexo == "hombre") echo "checked"; ?> value="hombre">Hombre
			<span class="error">* <?php echo $errorSexo; ?></span>

			<br><br>

			Aficiones: <br>
			<input type="checkbox" name="deportes" id="deportes" value="deportes">Deportes</label>
			<input type="checkbox" name="lectura" id="lectura" value="lectura">Lectura</label>
			<input type="checkbox" name="musica" id="musica" value="musica">Música</label>
			<input type="checkbox" name="cine" id="cine" value="cine">Cine</label>
			<input type="checkbox" name="idiomas" id="idiomas" value="idiomas">Idiomas</label>
			<span class="error">* <?php echo $errorAficiones; ?></span>

			<br><br>

			<input type="submit" name="submit" value="Enviar">
			<input type="reset" value="Limpiar">
		</form>

		<?php

		$pos = 0;

		echo "<h2>Salida de datos:</h2>";
		echo "Nombre: " . $nombre;
		echo "<br>";
		echo "Apellidos: " . $apellidos;
		echo "<br>";
		echo "Fecha de nacimiento: " . $fechaNac;
		echo "<br>";
		echo "Sueldo: " . $sueldo;
		echo "<br>";
		echo "Sexo: " . $sexo;
		echo "<br>";
		echo "Categoría: " . $categoria;

		$sumSueldos = 0;

		$personas = array(
			array(
				"Julio", "Rodríguez Márquez", "11/05/1989", "1600", "Peón", "Hombre", array("Deportes, Música")
			),
			array(
				"Marcos", "Alberca Sánchez", "04/10/1997", "2140", "Oficial", "Hombre", array("Lectura, Idiomas")
			),
			array(
				"Sara", "Martínez Abreu", "07/07/2003", "1301", "Director", "Mujer", array("Música, Cine")
			),
			array(
				"Rosalía", "Fernández Pérez", "22/12/1999", "3250", "Jefe de departamento", "Mujer", array("Lectura, Deportes")
			),
			array(
				"Carlos", "Salmerón Griñón", "11/11/2002", "1305", "Oficial", "Hombre", array("Deportes, Música")
			),
			array(
				"Daniel", "Marchena Jiménez", "01/01/1978", "2618", "Peón", "Mujer", array("Lectura, Música")
			),
			array(
				"Álvaro Manuel", "Martínez Molina", "03/06/1978", "950", "Jefe de departamento", "Hombre", array("Deportes, Idiomas")
			),
		);
		?>
	</div>
	<table>
		<tr>
			<th>Nombre</th>
			<th>Apellidos</th>
			<th>Fecha nacimiento</th>
			<th>Sueldo</th>
			<th>Profesión</th>
			<th>Sexo</th>
			<th>Aficiones</th>
		</tr>
		<?php
		foreach ($personas as $persona) {
			if ($persona[4] == "Peón") {
				echo "<tr style='background-color:#d3e36b'>";
			} else if ($persona[4] == "Oficial") {
				echo "<tr style='background-color:#41f05e'>";
			} else if ($persona[4] == "Jefe Departamento") {
				echo "<tr style='background-color:#e35fc0'>";
			} else {
				echo "<tr style='background-color:#5ac7e6'>";
			}
			echo "<td>";
			echo $persona[0];
			echo "</td>";
			echo "<td>";
			echo $persona[1];
			echo "</td>";
			echo "<td>";
			echo $persona[2];
			echo "</td>";
			echo "<td>";
			echo $persona[3];
			$sumSueldos = $sumSueldos + $persona[3];
			echo "</td>";
			echo "<td>";
			echo $persona[4];
			echo "</td>";
			echo "<td>";
			echo $persona[5];
			echo "</td>";
			echo "<td>";
			for ($i = 0; $i < count($persona[6]); $i++) {
				echo $persona[6][$i] . ", ";
			}
			echo "</td>";
			echo "</tr>";
		}
		echo "<tr>";
		echo "<td>";
		echo "</td>";
		echo "<td>";
		echo "</td>";
		echo "<td>";
		echo "Suma sueldos:";
		echo "</td>";
		echo "<td>";
		echo $sumSueldos;
		echo "</td>";
		?>
	</table>
</body>
</html>
